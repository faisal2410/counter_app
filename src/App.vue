<script setup>
import {ref} from "vue"

let count = ref(0)
</script>

<template>
  <main>
      <container class="container">
        <h2 >The current count is...</h2>
        <h1>{{count}}</h1>
        <button @click="count++">+</button>
        <button @click="count--">-</button>
      </container>
  </main>
</template>

<style scoped>
main {
  width: 100vw;
  height: 100vh;
  background-color: aliceblue;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'Montserrat', sans-serif;
}

.container {
  text-align: center;
}
</style>
