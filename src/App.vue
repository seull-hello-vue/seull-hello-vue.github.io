<script setup>
import { ref } from 'vew'
const count = ref(0)
</script>

<template>
<button @click="count++">Count is : {{ count }}</button>
</template>

<style scoped>
button{
font-weight: blod;
}
</style>
