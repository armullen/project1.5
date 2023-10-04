<template>
    <h1>All Dogs</h1>
    <div class="dogList">
      <dogCard class="dogCard" v-for="dog in dogs" :key="dog.id" :dog="dog" />
    </div>
  </template>
  
<script setup lang="ts">
import dogCard from "@/components/dogCard.vue";
import { ref } from "vue";

const dogs = ref([
    {name: "Spike", age: 5, breed: "Boxer", gender: "Male", id: 1}, 
    {name: "Rex", age: 3, breed: "Poodle", gender: "Male", id: 2},
    {name: "Rover", age: 2, breed: "Bulldog", gender: "Male", id: 3},
    {name: "Matilda", age: 3, breed: "Great Dane", gender: "Female", id: 4},
    {name: "Claire", age: 7, breed: "Bichon Frise", gender: "Female", id: 5},
    {name: "Phoebe", age: 1, breed: "Rottweiler", gender: "Female", id: 6}
]);

</script>
  <style scoped>
    .dogCard {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      border: solid black 2px;
    }
  
  </style>