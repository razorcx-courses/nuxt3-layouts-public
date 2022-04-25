<template>
  <div class="has-background-primary has-text-dark">
    <!-- <TheNav /> -->
    <header class="has-background-light has-text-dark">
      <slot name="header">Fallback header content</slot>
    </header>
    <main>
      <slot>Fallback main content</slot>
    </main>
    <footer class="has-background-link">
      <slot name="footer">Fallback footer content</slot>
    </footer>
  </div>
</template>

<script setup></script>

<style></style>
