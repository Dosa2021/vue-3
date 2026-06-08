<script setup>
const intro = 'フロントエンドエンジニア見習いです'; 
</script>

<template>
  <header>
    <p>
      <img src="/mei.webp" />
    </p>
    <h1>山田太郎</h1>
    <p v-text="intro"></p>
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
