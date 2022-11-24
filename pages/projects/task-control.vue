<template>
  <div>
    <NuxtLayout name="projects">
      <template #image>
        <img
          src="https://i.picsum.photos/id/20/3670/2462.jpg?hmac=CmQ0ln-k5ZqkdtLvVO23LjVAEabZQx2wOaT4pyeG10I"
          alt="side project image"
          class="md:w-8/12 m-auto my-20 contrast-50 brightness-50"
        />
      </template>

      <template #title>Tasks Control</template>
      <template #year>2022</template>

      <p class="leading-relaxed mb-6">
        Task Control is an application that allows you to control a list of
        tasks. You can add task with different fields such as dates, hours, etc.
        The application is able to count the number of hours you spend on each
        task. You can also search tasks by name. The goal of making this
        application was to create a way to track your tasks by hour and manage a
        database of data that persits accros the views.
      </p>

      <p class="leading-relaxed mb-6">
        I have decided to use Vue.js because it was one of the framework that I
        wanted to learn. I have also used Vuex to control the internal state of
        the application as well as Vue Router to create two different views. In
        the same way, I wanted to learn Tailwind CSS so the entire application
        is made with that framework. You can check the application
        <a
          href="https://fct-control-vuejs.netlify.app/"
          target="_blank"
          class="text-brand hover:text-brand-light transition duration-300 hover:underline"
          >in this link.</a
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
      tags: ["#Vue.js", "#Vuex", "#Vue Router", "#TailwindCSS"],
    };
  },
};
</script>
