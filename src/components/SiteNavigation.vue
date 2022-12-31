<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <header
    class="h-16 bg-teal-400 w-full flex items-center justify-center space-x-10"
  >
    <h1>{{ appTitle }}</h1>
    <RouterLink :to="{ name: 'home' }">Home</RouterLink>
    <RouterLink :to="{ name: 'shop' }">Shop</RouterLink>
  </header>
</template>

<script>
export default {
  data: () => {
    return {
      appTitle: import.meta.env.VITE_APP_TITLE,
    };
  },
};
</script>
