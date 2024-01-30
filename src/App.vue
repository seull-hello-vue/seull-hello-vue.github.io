<script setup>
import { ref } from 'vue'

const awesome = ref(true)

function toggleAwesome(v){
awesome.value = !v
}

function isAwesome(){
 return awesome.value

}



</script>

<template>
<button @click="toggleAwesome(awesome)">toggle</button>

<h1 v-if="isAwesome()">Vue is awesome!</h1>
<h1 v-else="toddleAwesome">NONONO</h1>

<h3 v-if="isAwesome"> v-if TRUE</h3>
<h3 v-show="isAwesome"> v-show TRUE</h3>

</template>
