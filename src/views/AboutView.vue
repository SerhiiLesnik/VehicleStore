<script setup lang="ts">
import { reactive } from 'vue';

const state = reactive({
  vehicleName: ''
});

function addVehicle(){
  alert(state.vehicleName)
}
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
    <input type="text" v-model="state.vehicleName">
    <button @click="addVehicle">Add vehicle</button>
  </div>
</template>

<style>

</style>
