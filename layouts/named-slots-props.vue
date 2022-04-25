<template>
  <div class="has-background-warning has-text-dark">
    <TheNav />
    <!-- Named Slot Props -->
    <header class="has-background-light has-text-dark">
      <slot name="header" :text="headerMessage"> Fallback header content </slot>
    </header>
    <main>
      <slot name="main" :text="mainMessage"> Fallback main content </slot>
    </main>
    <footer class="has-background-link has-text-light">
      <slot name="footer" :text="footerMessage"> Fallback footer content </slot>
    </footer>
  </div>
</template>

<script setup>
const headerMessage = ref();
headerMessage.value = "This is the header message using Named Slot Props";

const mainMessage = ref();
mainMessage.value = "This is the main message using Named Slot Props";

const footerMessage = ref();
footerMessage.value = "This is the footer message using Named Slot Props";
</script>

<style></style>
