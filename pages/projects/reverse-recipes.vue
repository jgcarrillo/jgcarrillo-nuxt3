<template>
  <div>
    <NuxtLayout name="projects">
      <template #image>
        <img
          src="/images/reverse-recipes.jpg"
          alt="side project image"
          class="md:w-8/12 m-auto my-20 contrast-50 brightness-50"
        />
      </template>

      <template #title>Reverse Recipes</template>
      <template #year>2021</template>

      <p class="leading-relaxed mb-6">
        Reverse Recipes is an application designed to search recipes by
        ingredients, which I have developed as my higher technician project. The
        objective was to get away from everything I had learned during the
        degree and learn technologies that really seemed interesting to me.
      </p>

      <p class="leading-relaxed mb-6">
        For its implementation I have decided to use Laravel and Vue.js with
        JetStream and Inertia and Tailwind CSS as style framework. If you are
        curious
        <a
          href="https://github.com/jgcarrillo/reverse-recipes/"
          target="_blank"
          class="text-brand hover:text-brand-light transition duration-300 hover:underline"
          >you can take a look here.</a
        >
      </p>

      <template #tags>
        <div v-for="tag in tags" :key="tag">
          <p
            class="text-sm lg:text-lg p-1 rounded-xl md:m-1 md:py-1 md:px-4 md:rounded-full text-white bg-brand"
          >
            {{ tag }}
          </p>
        </div>
      </template>
    </NuxtLayout>
  </div>
</template>

<script>
definePageMeta({
  layout: "false",
});

export default {
  data() {
    return {
      tags: ["#Laravel", "#Inertia", "#JetStream", "#TailwindCSS", "Vue.js"],
    };
  },
};
</script>
