<script setup>
const props = defineProps({
    imgUrl: String,
    title: String,
    desc: String
 });
</script>

<template>
    <section>
      <!-- <img :src="props.imgUrl" alt="すごい勇者ゲーム" width="500" /> -->
      <img :src="imgUrl" alt="すごい勇者ゲーム" width="500" />
      <h3>{{ title }}</h3>
      <p>{{ desc }}</p>
    </section>
</template>

<style scoped>
section {
  width: 400px;
  margin: 64px auto 0;
}

section p {
  margin-top: 16px;
  line-height: 1.8;
}
</style>