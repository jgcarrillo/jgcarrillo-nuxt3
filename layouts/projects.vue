<template>
  <div
    class="my-10 mx-10 md:my-20 md:mx-16 lg:my-20 lg:mx-20 xl:my-20 xl:mx-60 2xl:my-20 2xl:mx-96"
  >
    <div class="flex items-center justify-center">
      <NuxtLink to="/">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-12 h-12 text-gray-600 hover:text-gray-400 transition duration-500"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M19.5 12h-15m0 0l6.75 6.75M4.5 12l6.75-6.75"
          />
        </svg>
      </NuxtLink>
    </div>

    <slot />

    <TheFooter />
  </div>
</template>
