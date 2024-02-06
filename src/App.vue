<script setup>
  import { RouterLink, RouterView } from "vue-router";
  import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <header class="flex flex-col items-center p-6 tracking-widest">
    <img alt="Vue logo" class="logo" src="@/assets/logo.jpeg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav class="text-blue-600 font-semibold">
        <RouterLink to="/">Home</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>
