<script setup lang="ts">
import WorkSection from './WorkSection.vue';
const work_1 = {
  imgUrl: '/mei_1.jpg',
  titel: 'すごい勇者ゲーム',
  desc: 'すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。'
}

const works = [
  {
    imgUrl: '/mei_1.jpg',
    title: 'すごい勇者ゲーム',
    desc: 'すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。'
  },
  {
    imgUrl: '/mei_2.jpg',
    title: 'すごい勇者ゲーム-2',
    desc: 'すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。'
  },
  {
    imgUrl: '/mei_3.jpg',
    title: 'すごい勇者ゲーム-3',
    desc: 'すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。'
  }
]
</script>

<template>
  <main>
    <h2>WORKS</h2>
    <!-- <WorkSection v-bind="works[0]" /> -->
    <!-- <WorkSection v-bind="works[1]" /> -->
     <WorkSection v-for="work in works" v-bind="work"/>
  </main>
</template>

<style scoped>
main {
  padding: 64px 0;
}

h2 {
  margin: 0;
  font-weight: normal;
  font-size: 24px;
  text-align: center;
}

h3 {
  margin: 16px 0 0;
  font-weight: normal;
  font-size: 20px;
}
</style>