<template>
  <nav class="flex flex-row items-center justify-center md:text-lg">
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="/">
      <img src="~/assets/images/jgcarrillo.png" class="w-24 mx-10" />
    </NuxtLink>
    <NuxtLink to="/about">About</NuxtLink>
  </nav>
</template>

<style>
a.router-link-exact-active {
  color: #00cb8a;
  text-decoration: underline;
  text-underline-offset: 0.6em;
  text-decoration-thickness: 0.1em;
  text-decoration-color: #00cb8a;
}
</style>
