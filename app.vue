<template>
  <NuxtPage />
  <AuthOverlay v-if="isLoginOpen" />
  <!-- <AuthOverlay /> -->
</template>

<script setup>
import {storeToRefs} from 'pinia';

const {$generalStore} = useNuxtApp()
const { isLoginOpen } = storeToRefs($generalStore)
</script>