<script setup>
import PageB from './components/PageB.vue';
import PageA from './components/PageA.vue';
import { ref } from 'vue';

const a = ref('test');
</script>

<template>
  <div>

  </div>
  <PageA />
  <PageB />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
