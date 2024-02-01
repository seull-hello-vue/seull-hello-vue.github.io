<script setup>
import { ref } from 'vue'

const message = ref('')
</script>

<template>
<span>Multiline message is : </span>
<p style="white-spave: pre-line;">{{ message }}</p>
<textarea v-model="message" placeholder="add multiple line"></textarea>
</template>
