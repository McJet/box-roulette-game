<script setup>
import NavBar from './components/NavBar.vue';
</script>

<template>
  <div class="page">
    <NavBar v-bind:isLoggedIn="true" />
    <section class="main-view">

    </section>
  </div>
</template>

<style scoped>
.page {
  display: flex;
  flex-direction: column;
  justify-content: start;
  align-items: center;
}

.main-view {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
}
</style>
