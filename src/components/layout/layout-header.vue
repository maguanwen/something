<script setup lang="ts">
import { onMounted } from 'vue'
onMounted(() => {
const title = document.querySelector('.title')
if (title && title.textContent) {
  title.innerHTML = title.textContent
    .split('')
    .map((v) => `<span>${v}</span>`)
    .join('')
}
})
</script>

<template>
  <header>
    <div class="title">header</div>
  </header>
</template>

<style scoped lang="scss">
header {
  height: 120px;
  padding: 10px;
  background-color: black;
  color: #fff;
  .title {
    
    font-size: 80px;
    // font-style: italic;
    font-family: fantasy;
    letter-spacing: -8px;
  }
}
</style>
