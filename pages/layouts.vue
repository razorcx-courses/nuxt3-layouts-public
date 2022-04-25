<template>
  <div>
    <NuxtLayout>
      <div class="buttons is-flex is-justify-content-center my-4">
        <div class="button" @click="enableLayout('default')">Default</div>
        <div class="button" @click="enableLayout('custom')">Custom</div>
        <div class="button" @click="enableLayout('named-slots')">Named Slots</div>
        <div class="button" @click="enableLayout('named-slots-props')">Named Slot Props</div>
      </div>
      <div class="section">
          This is the page content
      </div>
    </NuxtLayout>
  </div>
</template>

<script setup>
const route = useRoute();

const enableLayout = (layout) => {
  route.meta.layout = layout;
};

//this turns off 'default' layout
//comment this out to use 'default' layout
definePageMeta({
  layout: false,
});
</script>

<style></style>
