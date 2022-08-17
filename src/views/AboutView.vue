<template>
  <div class="about">
    <h1> The number in the Home view was...</h1>
    <div class="number">{{storeCounter.count}}</div>
  </div>
</template>

<script setup>

import { useCounterStore } from '../stores/counter'

const storeCounter = useCounterStore();

</script> 

<style>
.about {
  width: 400px;
  height: 400px;
  margin: auto;
  padding-top: 50px;
  background-color: bisque;
  justify-content: center;
  padding: auto;
}
.number {
  margin: auto;
  margin-top: 100px;
  width: 200px;
  font-size: 80px;
  border: 2px solid grey
}
</style>