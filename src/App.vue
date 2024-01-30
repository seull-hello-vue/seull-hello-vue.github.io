<script setup>
import { ref } from 'vue'

const awesome = ref(true)
</script>

<template>
<button @click="awesome = !awesome">toggle</button>

<h1 v-if="awesome">Vue is awesome!</h1>
<h1 v-else>oh no T_T</h1>
<h2 v-if="awesome">true</h2>
<h2 v-show="awesome">TRUE</h2>
</template>
