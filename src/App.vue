<script setup>
import {ref} from 'vue'
let counter=ref(0)
console.log(counter)
const addToCounter=()=>{
counter.value=counter.value+1
console.log("HELLO FROM ADD TO COUNTER")
}
const decreaseCounter=()=>{
  console.log("HELLO FROM DECREASE")
  counter.value=counter.value-1
}

</script>

<template>
  <main>
  <div>
<h4>
  The current count is...
</h4>
<h1>{{ counter}}</h1>
<button @click="decreaseCounter">-</button>
<button @click="addToCounter">+</button>
</div>
</main>

  
</template>

<style scoped>
main {
  background-color: aliceblue;
  width: 100wh;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: space-around;
  text-align: center;
}

</style>
