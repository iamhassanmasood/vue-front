<script setup>
import WelcomeItem from './WelcomeItem.vue'

defineProps({
  randomMessage: {
    type: String,
    required: true
  }
})
</script>

<template>
  <WelcomeItem>
    <template #icon> </template>
    <template #heading>Documentation {{ randomMessage }}</template>
    <template #info>provides you with all information you need to get started. </template>
  </WelcomeItem>
</template>
