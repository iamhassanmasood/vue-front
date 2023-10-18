<script setup>
import WelcomeItem from './WelcomeItem.vue'

defineProps({
  docMessage: {
    type: String,
    required: true
  }
})
</script>

<template>
  <WelcomeItem>
    <template #heading>{{ docMessage }}</template>
    <template #info>provides you with all information you need to get started. </template>
  </WelcomeItem>
</template>
