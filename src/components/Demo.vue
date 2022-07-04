<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1>{{ msg }}</h1>
  <button type="button" class="btn" @click="count++">
    Count is: {{ count }}
  </button>
</template>

<style scoped>
.btn {
  font-size: 16px;
  color: white;
  border: 1px solid #ccc;
  background-color: #ccc;
  border-radius: 4px;
  padding: 5px 16px;
  cursor: pointer;
}
.btn:hover {
  background-color: #aaa;
}
</style>
