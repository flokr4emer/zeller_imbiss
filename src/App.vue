<script setup>
import { RouterView } from 'vue-router'
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue'
import TheScrollUpBtn from './components/TheScrollUpBtn.vue';
</script>

<template>
  <TheHeader />
  <RouterView />
  <TheFooter />
  <TheScrollUpBtn />
</template>

<style scoped></style>
