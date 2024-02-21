<script setup>
import { ref } from 'vue';

const count = ref(0);

const addCount = () => {
  count.value = count.value + 1;
}
const subCount = () => {
  count.value = count.value - 1;
}
</script>

<template>

  <main>
    <div>
      <h2>The current count is:</h2>
      <h1>{{ count }}</h1>
      <button @click="subCount">-</button>
      <button @click="addCount">+</button>
    </div>
  </main>
</template>

<style scoped>

  main {
    background-color: aliceblue;
    height: 100vh;
    width: 100vw;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  div {
    text-align: center;
  }


</style>
