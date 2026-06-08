<script setup>
import { ref } from 'vue';

const intro = 'フロントエンドエンジニア見習いです'; 
const imgUrl = '/mei.webp';
const count = ref(0)
const tags = [
  '#HTML',
  '#CSS',
  '#JavaScript'
]

function increment() {
  // count++
  count.value++
}
</script>

<template>
  <header>
    <p>
      <!-- <img src="/mei.webp" /> -->

      <!-- Note: v-bind -->
      <!-- <img v-bind:src="imgUrl" /> -->
      <img :src="imgUrl" />
    </p>
    <h1>山田太郎</h1>

    <!-- Note: v-text -->
    <p v-text="intro"></p>
    <!-- <p>{{ intro }}</p>
    <p>{{ intro.length }}</p> -->

    <!-- Note: v-on -->
    <!-- <button v-on:click="count++">いいね！（{{ count }}）</button> -->
    <!-- <button @click="count++">いいね！（{{ count }}）</button> -->
    <button @click="increment">いいね！（{{ count }}）</button>

    <!-- v-if -->
    <p v-if="count > 5">応援ありがとう</p>
    <p v-else>いいねお願いします</p>

    <!-- v-for -->
    <ul>
      <li v-for="tag in tags">{{ tag }}</li>
    </ul>
  </header>
</template>

<style scoped>
/* headerのスタイル */

header {
  background: #eee;
  text-align: center;
  padding: 32px 0;
  display: flex;
  flex-direction: column;
}

header img {
  border-radius: 50%;
}

h1 {
  margin: 16px 0 0;
  font-weight: normal;
  font-size: 24px;
}
</style>
