<template>
  <div>
    <NuxtLayout name="projects">
      <template #image>
        <img
          src="https://i.picsum.photos/id/201/5000/3333.jpg?hmac=NE8fOMa8u9PBfkq4AVwEoJdRqoPTNwUsyKvKWuXyNCk"
          alt="side project image"
          class="md:w-8/12 m-auto my-20 contrast-50"
        />
      </template>

      <template #title>Angular Cryptocurrency</template>
      <template #year>2021</template>

      <p class="leading-relaxed mb-6">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Consequatur
        magni, reprehenderit porro eius debitis laboriosam excepturi nobis
        mollitia nesciunt. Aliquid, tempore voluptatem. Veniam adipisci odit
        accusamus esse iste quibusdam quod! Lorem ipsum dolor sit amet
        consectetur adipisicing elit. Est sint unde minima amet voluptatum nobis
        mollitia porro sequi dolor! Sit rerum tenetur eaque possimus delectus
        quidem officiis vitae impedit accusantium. Lorem ipsum dolor, sit amet
        consectetur adipisicing elit. Ullam amet, ipsa ab exercitationem dicta,
        nihil quibusdam itaque saepe recusandae doloremque vero enim debitis
        possimus! Tempore minus debitis ea eligendi qui.
      </p>

      <p class="leading-relaxed mb-6">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Consequatur
        magni, reprehenderit porro eius debitis laboriosam excepturi nobis
        mollitia nesciunt. Aliquid, tempore voluptatem. Veniam adipisci odit
        accusamus esse iste quibusdam quod! Lorem ipsum dolor sit amet
        consectetur adipisicing elit. Est sint unde minima amet voluptatum nobis
        mollitia porro sequi dolor! Sit rerum tenetur eaque possimus delectus
        quidem officiis vitae impedit accusantium. Lorem ipsum dolor, sit amet
        consectetur adipisicing elit. Ullam amet, ipsa ab exercitationem dicta,
        nihil quibusdam itaque saepe recusandae doloremque vero enim debitis
        possimus! Tempore minus debitis ea eligendi qui.
      </p>

      <p class="leading-relaxed mb-6">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Consequatur
        magni, reprehenderit porro eius debitis laboriosam excepturi nobis
        mollitia nesciunt. Aliquid, tempore voluptatem. Veniam adipisci odit
        accusamus esse iste quibusdam quod! Lorem ipsum dolor sit amet
        consectetur adipisicing elit. Est sint unde minima amet voluptatum nobis
        mollitia porro sequi dolor! Sit rerum tenetur eaque possimus delectus
        quidem officiis vitae impedit accusantium. Lorem ipsum dolor, sit amet
        consectetur adipisicing elit. Ullam amet, ipsa ab exercitationem dicta,
        nihil quibusdam itaque saepe recusandae doloremque vero enim debitis
        possimus! Tempore minus debitis ea eligendi qui.
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
      tags: ["#Angular", "#API", "#Netlify", "#Fetch"],
    };
  },
};
</script>
