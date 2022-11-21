<template>
  <div>
    <h2
      class="text-2xl md:text-3xl text-center font-bold underline underline-offset-4 md:underline-offset-8 mb-14 md:mb-20"
    >
      Work experience
    </h2>

    <TheJob
      v-for="job in jobs"
      :key="job.id"
      :title="job.title"
      :link="job.link"
      :company="job.company"
      :duration="job.duration"
      :content="job.content"
    />
  </div>
</template>

<script>
import jobsList from "../data/jobs.json";

export default {
  data() {
    return {
      jobs: jobsList,
    };
  },
};
</script>
