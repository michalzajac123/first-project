<template>

  <HelloWorld v-for="number in numbers" />
  <button @click="add()" :style="{background:Kolor}">Dodaj</button>
  <input type="color" v-model="Kolor">
  {{ number }}
</template>

<script setup>
import HelloWorld from "./components/HelloWorld.vue";
import { ref } from "vue";
let Kolor=ref();
let number=ref(0);
let numbers=[2,3,4,5];

function add(){
  number.value++;
}

</script>

<style>

</style>
