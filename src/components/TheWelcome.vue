<script setup>
import WelcomeItem from './WelcomeItem.vue'

defineProps({
  welcomeMessage: {
    type: String,
    required: true
  }
})
</script>

<template>
  <WelcomeItem>
    <template #heading>Documentation {{ welcomeMessage }}</template>
    <template #info>provides you with all information you need to get started. </template>
  </WelcomeItem>
</template>
