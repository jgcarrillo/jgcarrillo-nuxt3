<template>
  <div class="mb-10 md:mb-12">
    <div class="mb-12 md:mb-14">
      <h3 class="text-xl md:text-2xl font-bold mb-2 md:mb-3">{{ title }}</h3>
      <a
        :href="link"
        class="text-brand hover:text-brand-light mb-2 text-xl"
        target="_blank"
        >{{ company }}</a
      >
      <p class="text-gray-400 font-thin mb-3 md:text-xl">
        {{ duration }}
      </p>
      <p class="leading-relaxed text-justify tracking-wide">
        {{ content }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["title", "link", "company", "content", "duration"],
};
</script>
