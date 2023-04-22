<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>

  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>

  
  <nav 
      class="
        flex-col
        mt-8
        space-y-4
        md:flex
        md:space-y-0
        md:flex-row
        md:items-center
        md:space-x-10
        md:mt-0
      ">
    <RouterLink class="text-sm font-bold text-gray-800 hover:text-blue-400" to="/">Home</RouterLink>
    <RouterLink class="text-sm font-bold text-gray-800 hover:text-blue-400" to="/project">project</RouterLink>
    <RouterLink class="text-sm font-bold text-gray-800 hover:text-blue-400" to="/skill">skill</RouterLink>
    <RouterLink class="text-sm font-bold text-gray-800 hover:text-blue-400" to="/experience">experience</RouterLink>
  </nav>
  <RouterView />
</template>