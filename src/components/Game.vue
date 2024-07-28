<script setup>
import { ref } from "vue";
import Scoreboard from "./Scoreboard.vue";
import BoxContainer from "./BoxContainer.vue";

const box1Content = ref("🎁");
const box2Content = ref("🎁");
const box3Content = ref("🎁");
const box4Content = ref("🎁");
</script>

<template>
  <div class="game">
    <Scoreboard :moneyAmount="1000" :boxesAmount="0" />
    <BoxContainer
      :box1Content="box1Content"
      :box2Content="box2Content"
      :box3Content="box3Content"
      :box4Content="box4Content"
    />
  </div>
</template>

<style scoped>
.game {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  gap: 10dvh;
  padding: 10dvh 0;
  width: 100%;
  height: 100%;
  max-height: 950px;
  @media (min-width: 768px) {
    max-height: 1000px;
  }
}
</style>
