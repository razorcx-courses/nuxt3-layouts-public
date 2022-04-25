<template>
  <NuxtLayout name="common">
    <TheHero />
    <div class="container">
      <TheContent :text="content" class="box p-6 m-6" />
    </div>
  </NuxtLayout>
</template>

<script setup>
const content = ref();
content.value = "About page content";
</script>

<style></style>
