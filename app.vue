<template>
  <div>
    <!-- <NuxtWelcome /> -->

    <NuxtLayout></NuxtLayout>
  </div>
</template>
<script setup>
useHead({
  title: "Ecommerce",
  // or, instead:
  // titleTemplate: (title) => `My App - ${title}`,
  viewport: "width=device-width, initial-scale=1, maximum-scale=1",
  charset: "utf-8",
  meta: [{ name: "description", content: "My amazing site ecommerce" }],
  // bodyAttrs: {
  //   class: 'test'
  // }
});
</script>
