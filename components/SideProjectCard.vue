<template>
  <a
    :href="url"
    class="rounded overflow-hidden shadow-lg hover:scale-105 transition duration-300"
  >
    <nuxt-img :src="image" alt="side project image" class="w-full" />
    <div class="text-center p-6">
      <h3 class="sm:text-normal md:text-xl lg:text-2xl font-bold mb-2">
        {{ title }}
      </h3>
      <p class="sm:text-sm md:text-xl text-gray-400 font-thin sm:mb-2 md:mb-3">
        {{ subtitle }}
      </p>
    </div>
  </a>
</template>

<script>
export default {
  props: ["title", "subtitle", "image", "url"],
};
</script>
