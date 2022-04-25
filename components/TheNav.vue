<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <NuxtLink class="navbar-item" href="/">
        <h1 class="title is-5">Nuxt3Layouts</h1>
      </NuxtLink>
    </div>

    <div id="navbar" class="navbar-menu">
      <div class="navbar-start">
        <NuxtLink class="navbar-item" to="/about"> About </NuxtLink>
        <NuxtLink class="navbar-item" to="/contact"> Contact </NuxtLink>
        <NuxtLink class="navbar-item" to="/layouts"> Layouts </NuxtLink>
      </div>
    </div>
  </nav>
</template>

<script setup></script>

<style></style>
