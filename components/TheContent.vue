<template>
  <div>
    <h2 class="section p-4 my-3 is-size-4">{{ text }}</h2>
  </div>
</template>

<script setup>
const props = defineProps({
  text: String,
});
</script>

<style></style>
