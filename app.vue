<template>
  <NuxtPage />
  <AuthOverlay v-if="isLoginOpen" />
  <EditProfileOverlay v-if="isEditProfileOpen" />
  <!-- <AuthOverlay /> -->
</template>

<script setup>
import {storeToRefs} from 'pinia';

const {$generalStore} = useNuxtApp()
const { isLoginOpen, isEditProfileOpen } = storeToRefs($generalStore)
</script>