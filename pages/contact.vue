<template>
  <NuxtLayout name="named-slots">
    <!-- header slot -->
    <template #header>
      <TheHero />
    </template>

    <!-- implicit default slot -->
    <div class="container">
      <TheContactForm class="section p-6" />
    </div>

    <!-- footer slot -->
    <template #footer>
      <TheFooter />
    </template>
  </NuxtLayout>
</template>

<script>
export default {};
</script>

<style></style>
