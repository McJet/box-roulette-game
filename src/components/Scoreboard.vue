<script setup>
import { ref } from "vue";

const props = defineProps({
  moneyAmount: Number,
  boxesAmount: Number,
});
// add commas to the amounts
const formattedMoneyAmount = ref(props.moneyAmount.toLocaleString());
const formattedBoxesAmount = ref(props.boxesAmount.toLocaleString());
</script>

<template>
  <div class="scoreboard">
    <div class="inner">
      <p class="label">Money Earned</p>
      <p>${{ formattedMoneyAmount }}</p>
    </div>
    <div class="line"></div>
    <div class="inner">
      <p class="label">Boxes Opened</p>
      <p>{{ formattedBoxesAmount }}</p>
    </div>
  </div>
</template>

<style scoped>
.scoreboard {
  display: flex;
  justify-content: center;
  gap: 1em;
  font-size: calc(10px + 2vmin);
}
.inner {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.label {
  font-weight: bold;
}
.line {
  width: 1px;
  background-color: white;
}
</style>
