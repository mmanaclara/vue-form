<script setup>
import { RouterView } from 'vue-router'
import MovingTruckIcon from './components/icons/IconMovingTruck.vue'
</script>

<template>
  <main class="maxAd">
    <div class="wrapper">
      <MovingTruckIcon />
      <h1>Max Mudanças</h1>
      <span>Sua empresa de mudanças 24h. Conte com a gente para iniciar essa nova fase com o pé direito!</span>
    </div>
  </main>

  <RouterView />
</template>

<style scoped>
.maxAd {
  width: 70%;
  background: hsla(160, 100%, 37%, 1);
  color: black;
}

.maxAd h1 {
  font-weight: bold;
  font-style: italic;
  font-size: x-large;
  margin-bottom: 6px;
}
.wrapper {
  width: 60%;
  margin-inline: auto;
  height: 100vh;
  text-align: center;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>