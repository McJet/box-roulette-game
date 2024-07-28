<script setup>
import NavBar from "./components/NavBar.vue";
import Game from "./components/Game.vue";
</script>

<template>
  <div class="page">
    <NavBar v-bind:isLoggedIn="true" />
    <section class="main-view">
      <Game />
    </section>
  </div>
</template>

<style scoped>
.page {
  display: flex;
  flex-direction: column;
  justify-content: start;
  align-items: center;
  width: 100dvw;
  height: 100dvh;
}

.main-view {
  display: flex;
  flex-direction: column;
  justify-content: start;
  align-items: center;
  width: 100%;
  height: 100%;
}
</style>
