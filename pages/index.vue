<template>
  <div>
    <TheNav />

    <NuxtLayout name="default" class="section">
      <h2 class="card p-4 my-3 is-size-4">Page with Default Layout</h2>
    </NuxtLayout>

    <NuxtLayout name="custom" class="section">
      <h2 class="card p-4 my-3 is-size-4">Page with Custom Layout</h2>
    </NuxtLayout>

    <NuxtLayout name="named-slots" class="section">
      <!-- header slot -->
      <template #header>
        <p>Header</p>
        <p>This is the Header without props</p>
      </template>

      <!-- implicit default slot -->
      <h2 class="card p-4 my-3 is-size-4">Page with Named Slots</h2>

      <!-- footer slot -->
      <template #footer>
        <p>Footer</p>
        <p>This is the footer without props</p>
      </template>
    </NuxtLayout>

    <NuxtLayout name="named-slots-props" class="section">
      <!-- header slot -->
      <template #header="headerProps">
        <p>Header</p>
        <p>{{ headerProps.text }}</p>
      </template>

      <template #main="mainProps">
        <h2 class="card p-4 my-3 is-size-4">{{ mainProps.text }}</h2>
      </template>

      <!-- footer slot -->
      <template #footer="footerProps">
        <p>Footer</p>
        <p>{{ footerProps.text }}</p>
      </template>
    </NuxtLayout>
  </div>
</template>

<script setup></script>

<style></style>
