<template>
  <section class="bg-gray-700 py-20 mb-4">
    <div :class="heroStyles">
      <h1 :class="h1Styles">
        {{ title }}
      </h1>
      <p class="my-4 text-xl text-white">{{ subtitle }}</p>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';
const heroStyles = ref(
  `max-w-7xl mx-auto 
   px-4 sm:px-6 lg:px-8 
   flex flex-col 
   items-center text-center`,
);

const h1Styles = ref(`
  text-4xl font-extrabold 
  text-white sm:text-5xl 
  md:text-6xl`);

defineProps({
  title: {
    type: String,
    default: 'Search for developer careers',
  },
  subtitle: {
    type: String,
    default: 'Find a career that fits your skills and needs',
  },
});
</script>

<style lang="scss" scoped></style>
