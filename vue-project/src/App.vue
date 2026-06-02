<script setup>
import Header from "./components/Header.vue";
</script>

<template>
  <Header />
  <main>
    <h2>WORKS</h2>
    <section>
      <img src="" alt="すごい勇者ゲーム" width="400" height="240" />
      <h3>すごい勇者ゲーム</h3>
      <p>
        すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。すごい勇者ゲームです。
      </p>
    </section>
    <section>
      <img src="" alt="すごい宝物ゲーム" width="400" height="240" />
      <h3>すごい宝物ゲーム</h3>
      <p>
        すごい宝物ゲームです。すごい宝物ゲームです。すごい宝物ゲームです。すごい宝物ゲームです。すごい宝物ゲームです。すごい宝物ゲームです。すごい宝物ゲームです。
      </p>
    </section>
    <section>
      <img src="" alt="すごいカードゲーム" width="400" height="240" />
      <h3>すごいカードゲーム</h3>
      <p>
        すごいカードゲームです。すごいカードゲームです。すごいカードゲームです。すごいカードゲームです。すごいカードゲームです。すごいカードゲームです。すごいカードゲームです。
      </p>
    </section>
  </main>
  <footer>
    <small>(c) dotinstall.com</small>
  </footer>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
