<script setup>
import { ref,onMounted } from 'vue'

//reactive state
const count = ref(0)

function increment(){
count.value = count.value+1
//count.value++
}

 function increment1(){
   count.value--
  }

//lifecycle hooks
onMounted(() => {
console.log('The initial count is ${count.value}.')
})

</script>

<template>
<button @click="increment">UP</button>
<button @click="increment">Count is : {{ count }}</button>
<button @click="increment1">Down</button>
</template>
<style scoped>
button{
font-weight: blod;
width: 100px;
height : 50px;
background : yellow;
}
</style>
