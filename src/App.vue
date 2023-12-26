<template>
  <input />
  <!-- focus goes to second input -->
  <input ref="input" />
</template>

<script setup>
import { ref, onMounted } from "vue";

const input = ref(null);

onMounted(() => {
  // it goes becaus of this code
  input.value.focus();
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
