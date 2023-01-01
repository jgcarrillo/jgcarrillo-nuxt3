<template>
  <div>
    <NuxtLayout name="projects">
      <template #image>
        <img
          src="/images/telegram-bot.jpg"
          alt="side project image"
          class="md:w-8/12 m-auto my-20 contrast-50 brightness-50"
        />
      </template>

      <template #title>Telegram Bot</template>
      <template #year>2022</template>

      <p class="leading-relaxed mb-6">
        Telegram Bot is an application I have built for my family and friends in
        my spare time for two weeks. It has been developed, above all, to
        experiment with Telegram bots. The goal was to build a simple weather
        bot, to check the currect weather and forecast for five days. It also
        allows users to create reminders and list them.
      </p>

      <p class="leading-relaxed mb-6">
        For its implementation, I have decided to use a library called grammY to
        communicate wit the Telegram API as well as TypeScript and Axios to make
        requests to weather API. I have also contributed to this library adding
        the Vercel documentation to deploy the bot. It was an incredible project
        with great challenges that I had to overcome.
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
      tags: ["#TypeScript", "#grammY", "#Axios", "#Vercel"],
    };
  },
};
</script>
