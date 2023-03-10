<script setup>
import HeroItem from '../components/HeroItem.vue'
import img from '../assets/MenuHeroImg.jpg'
</script>


<template>
    <HeroItem :src="img" />
</template>

<script>
export default {
    name: "MenuView",
}
</script>

<style scoped></style>