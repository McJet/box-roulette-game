<script setup>
import { ref } from "vue";

const props = defineProps({});
</script>

<template>
  <button class="box">
    <slot></slot>
  </button>
</template>

<style scoped>
.box {
  background-color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  border-radius: 24px;

  color: black;
  font-size: 96px;
}
</style>
