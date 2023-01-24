<template>
  <div>
    <h2
      class="text-2xl md:text-2xl text-center font-bold underline underline-offset-4 md:underline-offset-8 mb-14 md:mb-20"
    >
      Tech Talks
    </h2>

    <TheTalk
      v-for="talk in talks"
      :key="talk.id"
      :title="talk.title"
      :link="talk.link"
      :location="talk.location"
      :datetime="talk.datetime"
      :icon="talk.icon"
    />
  </div>
</template>

<script>
import talksList from "../data/talks.json";

export default {
  data() {
    return {
      talks: talksList,
    };
  },
};
</script>
