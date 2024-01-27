<script setup lang="ts">
  import Header from "../components/header/Header.vue";
</script>

<template>
  <div class="contact">
    <Header></Header>
  </div>
</template>

<style scoped>
@media (min-width: 1024px) {
  .contact {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>