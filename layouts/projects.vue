<template>
  <div
    class="my-10 mx-10 md:my-20 md:mx-16 lg:my-20 lg:mx-20 xl:my-20 xl:mx-60 2xl:my-20 2xl:mx-96"
  >
    <!-- Arrow icon -->
    <div class="flex items-center justify-center">
      <NuxtLink to="/">
        <IconsArrowIcon />
      </NuxtLink>
    </div>

    <!-- Image with title and year -->
    <div class="relative">
      <slot name="image" />
      <div
        class="flex flex-col justify-center items-center absolute w-full h-full top-0 right-0 text-white"
      >
        <h1 class="text-normal md:text-3xl font-bold mb-2">
          <slot name="title"></slot>
        </h1>
        <h2 class="text-normal md:text-2xl font-thin">
          <slot name="year"></slot>
        </h2>
      </div>
    </div>

    <!-- Content -->
    <div>
      <h2
        class="text-2xl md:text-2xl text-center font-bold underline underline-offset-4 md:underline-offset-8 mb-14 md:mb-20"
      >
        Description
      </h2>

      <!-- Main content (text) -->
      <slot />

      <div class="my-20">
        <h2
          class="text-2xl md:text-2xl text-center font-bold underline underline-offset-4 md:underline-offset-8 mb-14 md:mb-20"
        >
          Tech used
        </h2>
        <div class="flex flex-row flex-wrap justify-center gap-2">
          <!-- Tags (technologies) -->
          <slot name="tags"></slot>
        </div>
      </div>
    </div>

    <TheFooter />
  </div>
</template>
