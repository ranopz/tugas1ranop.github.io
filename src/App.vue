<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <nav class="text-center py-10">
      <RouterLink class="bg-gray-100 rounded-lg border border-none text-sm p-2.5 text-black mr-2 hover:bg-teal-500 font-medium" to="/" > home </RouterLink>
      <RouterLink class="bg-gray-100 rounded-lg border border-none text-sm p-2.5 text-black mr-2 hover:bg-teal-500 font-medium" to="/myapp" > aplikasi </RouterLink>
      <RouterLink class="bg-gray-100 rounded-lg border border-none text-sm p-2.5 text-black mr-2 hover:bg-teal-500 font-medium" to="/about" > about </RouterLink>
    </nav>
  </header>
<RouterView class="pt-20" />
</template>

<style>
nav a.router-link-exact-active {
  @apply bg-teal-600;
  @apply text-white;
}
</style>