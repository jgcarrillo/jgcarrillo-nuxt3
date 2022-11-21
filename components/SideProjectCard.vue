<template>
  <a
    href="/"
    class="rounded overflow-hidden shadow-lg hover:scale-105 transition duration-300"
  >
    <img :src="image" alt="side project image" class="w-full" />
    <div class="text-center p-6">
      <h3 class="text-xl md:text-2xl font-bold mb-2">{{ title }}</h3>
      <p class="text-gray-400 font-thin mb-2 md:mb-3 md:text-xl">
        {{ subtitle }}
      </p>
    </div>
  </a>
</template>

<script>
export default {
  props: ["title", "subtitle", "image"],
};
</script>
