<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
const viteUrl = 'https://vitejs.dev/'
const vueUrl = 'https://vuejs.org/'
</script>

<template>
  <div>
    <h1>{{ msg }}</h1>
    <h3>
      <a v-bind:href="viteUrl" target="_blank" rel="noopener">Vite</a> +
      <a v-bind:href="vueUrl" target="_blank" rel="noopener">Vue 3</a>.
    </h3>
  </div>
</template>
