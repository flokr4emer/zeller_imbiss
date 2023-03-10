<script setup>
import HeroItem from '../components/HeroItem.vue'
import img from '../assets/CartHeroImg.jpg'
</script>


<template>
    <HeroItem :src="img" />
</template>

<script>

export default {
    name: "CartVue",
    data() {
        return {

        };
    },
}
</script>

<style scoped></style>