<script setup>
  // Importing the reactive function from Vue
  import { ref, watchEffect, onMounted } from "vue";

  // Ui Components
  import { Input } from "@/components/ui/input";
  import { Trash2 } from "lucide-vue-next";
  import { Button } from "@/components/ui/button";
  import { Card, CardContent, CardFooter } from "@/components/ui/card";
  import { FormField, FormControl, FormItem, FormLabel, FormMessage } from "@/components/ui/form";

  // Form validations
  import { toTypedSchema } from "@vee-validate/zod";
  import { useForm } from "vee-validate";
  import * as z from "zod";

  const formSchema = toTypedSchema(
    z.object({
      todo: z.string().min(2).max(50), // Validating the todo field
    })
  );
  const form = useForm({
    validationSchema: formSchema,
  });

  // Reactive state for todos
  const todos = ref([]);

  // Load todos from local storage
  const loadTodos = () => {
    const storedTodos = localStorage.getItem("todos");
    if (storedTodos) {
      todos.value = JSON.parse(storedTodos);
    }
  };

  // Watch for changes in todos and save them to local storage
  watchEffect(() => {
    localStorage.setItem("todos", JSON.stringify(todos.value));
  });

  onMounted(() => {
    loadTodos(); // Mounting loadTodos to initialize the state from local storage
  });

  const onSubmit = form.handleSubmit((values) => {
    // Add the new todo to the todos array
    todos.value.push(values.todo);

    // Clear the form field after submission
    form.resetForm();
  });
</script>

<template>
  <main class="px-64 space-y-6">
    <form @submit="onSubmit" class="space-y-5">
      <FormField v-slot="{ componentField }" name="todo">
        <FormItem>
          <FormLabel>Enter your to do here:</FormLabel>
          <FormControl>
            <Input type="text" placeholder="Learning VueJs Today" v-bind="componentField" />
          </FormControl>
          <FormMessage />
        </FormItem>
      </FormField>
      <Button type="submit">Submit</Button>
    </form>

    <div v-if="todos.length === 0" class="text-xl">No todos found.</div>

    <div v-for="(todo, index) in todos" :key="index">
      <Card class="flex items-center pt-6 justify-between">
        <CardContent class="text-xl">{{ todo }}</CardContent>
        <CardFooter class="space-x-5">
          <Button @click="todos.splice(index, 1)"> <Trash2 /></Button>
        </CardFooter>
      </Card>
    </div>
  </main>
</template>
