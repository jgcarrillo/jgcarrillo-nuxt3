<template>
  <div>
    <NuxtLayout name="projects">
      <template #image>
        <img
          src="/images/angular-crypto.jpg"
          alt="side project image"
          class="md:w-8/12 m-auto my-20 contrast-50 brightness-50"
        />
      </template>

      <template #title>Angular Cryptocurrency</template>
      <template #year>2021</template>

      <p class="leading-relaxed mb-6">
        Angular Cryptocurrency is an application designed to show a list of
        cryptos which I have developed to improve my Angular Skills. The
        objective was to use an API, get the data and let the user to search for
        crypto by name and even add the currency to a favorite place. Once the
        crypto is there, you can also see the details fot it.
      </p>

      <p class="leading-relaxed mb-6">
        It's implementation its very simple since I have only used Angular with
        BootStrap. You can check the application
        <a
          href="https://angular-crypto-api.netlify.app/"
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
      tags: ["#Angular", "#API", "#Netlify", "#Fetch", "#BootStrap"],
    };
  },
};
</script>
