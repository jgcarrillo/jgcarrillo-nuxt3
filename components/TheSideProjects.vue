<template>
  <div class="mb-16 md:mb-20">
    <h2
      class="text-2xl md:text-2xl text-center font-bold underline underline-offset-4 md:underline-offset-8 mb-14 md:mb-20"
    >
      Side projects
    </h2>

    <div
      class="grid grid-cols-1 md:grid-cols-2 gap-5 md:gap-7 m-4 md:m-14 lg:m-24"
    >
      <SideProjectCard
        v-for="project in projects"
        :key="project.id"
        :title="project.title"
        :subtitle="project.subtitle"
        :image="project.image"
        :url="project.url"
      />
    </div>
  </div>
</template>

<script>
import sideProjects from "../data/side.json";

export default {
  data() {
    return {
      projects: sideProjects,
    };
  },
};
</script>
