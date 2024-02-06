<script setup>
  defineProps({
    msg: {
      type: String,
      required: true,
    },
  });
</script>

<template>
  <div class="">
    <h1 class="">{{ msg }}</h1>
    <h3>Welcome to VueJs Workshop!</h3>
  </div>
</template>
