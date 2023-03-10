<script setup>
//
</script >

<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-12">
                <img class="img-fluid" :src="src" :alt="alt">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "HeroItem",
    props: {
        src: {
            type: Object,
            required: true,
        },
        alt: {
            type: String,
            default: "Picture"
        }
    },
}
</script>

<style scoped>
.container {
    margin: 0;
    padding: 0;
}
</style>