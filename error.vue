<template>
  <NuxtLayout name="default">
    <div class="m-12 md:m-20">
      <h1 class="text-4xl md:text-6xl font-bold text-center">404, but...</h1>
      <p class="my-6 text-xl md:text-2xl font-thin text-center">
        Yeah... that was embarrasing. But I encourage you to check any of the
        sections of the web. Maybe you will find out something interesting!
      </p>
    </div>
  </NuxtLayout>
</template>

<script>
export default {
  methods: {
    handleError() {
      clearError({ redirect: "/" });
    },
  },
};
</script>
