<script setup>


import category from "@/assets/category.json"

const categories = category
</script>

<template>


<h1 v-for="item in categories">
  name : {{ item.name }}  
  code : {{ item.code }}
 </h1>
</template>
