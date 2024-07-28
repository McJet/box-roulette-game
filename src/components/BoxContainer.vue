<script setup>
import Box from "./Box.vue";

const props = defineProps({
  box1Content: String,
  box2Content: String,
  box3Content: String,
  box4Content: String,
});
</script>

<template>
  <div class="box-container">
    <Box>{{ box1Content }}</Box>
    <Box>{{ box2Content }}</Box>
    <Box>{{ box3Content }}</Box>
    <Box>{{ box4Content }}</Box>
  </div>
</template>

<style scoped>
.box-container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, 1fr);
  height: calc(1dvh - 50px);
  gap: 1em;
  width: 90vw;
  height: 90vw;
  max-width: 500px;
  max-height: 500px;
}
</style>
