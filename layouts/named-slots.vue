<template>
  <div class="has-background-primary has-text-dark">
    <!-- <TheNav /> -->
    <header class="has-background-light has-text-dark">
      <slot name="header"></slot>
    </header>
    <main>
      <slot></slot>
    </main>
    <footer class="has-background-link">
      <slot name="footer"></slot>
    </footer>
  </div>
</template>

<script setup></script>

<style></style>
