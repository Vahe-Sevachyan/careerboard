<template>
  <nav class="bg-gray-700 border-b border-gray-500">
    <div :class="navStyles">
      <!-- Logo -->
      <a class="flex shrink-0 items-center mr-4" href="index.html">
        <img class="h-10 w-auto" :src="logo" alt="Vue Jobs" />
        <span class="hidden md:block text-white text-2xl font-bold ml-2">Career Board</span>
      </a>

      <div class="flex space-x-2 md:ml-auto items-center">
        <a
          href="index.html"
          class="text-white bg-gray-900 hover:bg-gray-800 hover:text-white rounded-md px-3 py-2"
          >Home</a
        >
        <a
          href="jobs.html"
          class="text-white hover:bg-gray-800 hover:text-white rounded-md px-3 py-2"
          >Jobs</a
        >
        <a
          href="add-job.html"
          class="text-white hover:bg-gray-800 hover:text-white rounded-md px-3 py-2"
          >Add Job</a
        >
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue';
import logo from '../assets/img/logo.png';
const navStyles = ref(
  `mx-auto px-2 sm:px-6 lg:px-8 
   max-w-7xl flex flex-1 
   items-center h-20 justify-center 
   md:items-stretch md:justify-start
   `,
);
</script>

<style lang="css" scoped></style>
