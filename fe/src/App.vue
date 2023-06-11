<script setup lang="ts">

  async function log() {
    const response = fetch('/api');
    const msg = (await response).text();
    console.log(msg)
  }

</script>

<template>
  <button @click="log">Click</button>
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
