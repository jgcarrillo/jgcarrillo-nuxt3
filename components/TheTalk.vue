<template>
  <div class="mb-10 md:mb-12">
    <div class="mb-12 md:mb-7">
      <a
        :href="link"
        class="talk-title-container text-brand hover:text-brand-light text-xl"
        target="_blank"
      >
        <img :src="`/images/${icon}`" alt="talk logo" class="talk-logo" />
        <h3 class="font-bold mb-2">{{ title }}</h3>
      </a>
      <p class="text-gray-400 font-thin mb-2 md:text-xl">
        {{ location }}
      </p>
      <p class="text-gray-400 font-thin">
        {{ datetime }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["title", "link", "location", "datetime", "icon"],
};
</script>

<style scoped>
.talk-title-container {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  width: -webkit-fit-content;
  width: -moz-fit-content;
  width: fit-content;
  margin-bottom: 0.5rem;
}
.talk-logo {
  width: 24px;
  height: 24px;
  margin-right: 8px;
}
</style>
