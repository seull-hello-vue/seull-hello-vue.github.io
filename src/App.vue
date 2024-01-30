<script setup>

import { ref } from 'vue'
import category from "@/assets/gamelist.json"

const categories = ref(category)
const awesome = ref(true)


</script>

<template>

<h1>게임플레이타임 100분이상 출력하기</h1>

<dev v-for="item in categories">
<li v-if="item.playtime_forever > 100">
게임이름 : {{ item.name }} <br>
  나의 플레이 시간 : {{item.playtime_forever}} 분
</li>
</dev>
</template>
