<script setup>
import HeroItem from "../components/HeroItem.vue";
import img from "../assets/AboutHeroImg.jpg"
</script>

<template>
  <HeroItem :src="img" />
</template>

<script>
export default {
  name: "AboutView",
}
</script>


<style></style>
