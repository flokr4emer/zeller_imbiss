<template>
    <button class="btn">^</button>
</template>

<script>
export default {
    name: "TheScrollUpBtn",
}
</script>

<style scoped>
.btn {
    background-color: brown;
    position: fixed;
    bottom: 20px;
    right: 30px;
    z-index: 99;
    border: none;
    outline: none;
    color: white;
    padding: 15px 23px 15px 23px;
    border-radius: 10px;
    font-size: 18px;
}

.btn:hover {
    background-color: brown;
    color: white;
}
</style>
