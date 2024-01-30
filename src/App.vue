<script setup>

import { ref } from 'vue'
import category from "@/assets/gamelist.json"

const categories = ref(category)
const awesome = ref(true)


</script>

<template>

<h1>나의 플레이타임 100분 이상 출력하기!</h1>
<br><br><br>
<ul v-for="item in categories">
<li v-if="item.playtime_forever > 100">
게임이름 : {{ item.name }} <br>
나의 플레이 시간 : {{item.playtime_forever}} 분<br>
</li>
</ul>
</template>
