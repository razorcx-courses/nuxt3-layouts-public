<template>
  <div class="has-background-warning has-text-dark">
    <!-- Names Slot Props -->
    <header class="has-background-light has-text-dark">
      <slot name="header" :text="headerMessage"></slot>
    </header>
    <main>
      <slot name="main" :text="mainMessage"></slot>
    </main>
    <footer class="has-background-link has-text-light">
      <slot name="footer" :text="footerMessage"></slot>
    </footer>
  </div>
</template>

<script setup>
const headerMessage = ref();
headerMessage.value = "This is the header message using Named Slot Props"

const mainMessage = ref();
mainMessage.value = "This is the main message using Named Slot Props"

const footerMessage = ref();
footerMessage.value = "This is the footer message using Named Slot Props"
</script>

<style></style>
