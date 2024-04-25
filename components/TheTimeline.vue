<template>
  <div>
    <h1 class="md:text-3xl text-2xl font-bold">Timeline</h1>
    <div v-for="entry in timelineData" :key="entry.year">
      <h2 class="mt-4 md:text-2xl text-xl font-bold">{{ entry.year }}</h2>
      <ol class="relative border-s border-green-200 m-4">
        <li
          class="mb-5 ms-4"
          v-for="(item, index) in entry.entries"
          :key="index"
        >
          <div
            class="absolute w-3 h-3 bg-green-400 rounded-full mt-2 -start-1.5 bg-gradient-to-r from-green-400 to-green-500"
          ></div>
          <h3 class="md:text-lg text-md font-semibold text-gray-900">
            {{ item.title }}
          </h3>
          <p class="md:text-base text-base text-gray-500">
            {{ item.description }}
          </p>
        </li>
      </ol>
    </div>
  </div>
</template>

<script>
import timelineData from "../data/timeline.json";

export default {
  data() {
    return {
      timelineData,
    };
  },
};
</script>
