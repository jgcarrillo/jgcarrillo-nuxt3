<template>
  <nav class="flex flex-row items-center justify-center md:text-lg">
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="/">
      <img
        src="/images/jgcarrillo.png"
        class="mx-4 w-16 md:w-24 md:mx-10 hover:brightness-105 transition duration-300"
      />
    </NuxtLink>
    <NuxtLink to="/about">About</NuxtLink>
  </nav>
</template>

<style scoped>
a.router-link-exact-active {
  color: #00cb8a;
  text-decoration: underline;
  text-underline-offset: 0.6em;
  text-decoration-thickness: 0.1em;
  text-decoration-color: #00cb8a;
}
a:hover {
  color: #00cb8a;
  transition: 300ms;
}
</style>
