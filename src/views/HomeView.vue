<template>
  <div class="home">
      <div class="counter">
      {{ storeCounter.count }}
    </div>
    <div class="buttons">
      <button @click="storeCounter.decreaseCount">-</button>
      <button @click="storeCounter.increaseCount">+</button>
    </div>
    <hr/>
    <div>
      Now it's an {{storeCounter.isOddOrEven}} number!
    </div>
    <hr/>
    <div>
      <h3>Edit Counter</h3>
      <input v-model="storeCounter.count" type="number">
    </div>
  </div>
</template>

<script setup>

import { useCounterStore } from '@/stores/counter'

const storeCounter = useCounterStore();

</script>

<style>
hr {
  width: 160px;
}

.home {
  width: 400px;
  height: 400px;
  margin: auto;
  padding-top: 50px;
  background-color: bisque;
  justify-content: center;
  padding: auto;
}

.counter {
  font-size: 60px;
  margin: 20px;
}

.buttons button {
  font-size: 40px;
  margin: 10px;
}
</style>