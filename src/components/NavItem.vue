<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
    <li class="nav-item">
        <RouterLink :to="to" class="nav-link" :linkName="linkName">{{ linkName }}</RouterLink>
    </li>
</template>

<script>
export default {
    name: "NavItem",
    props: {
        linkName: {
            type: String,
            required: true
        },
        to: {
            type: String,
            required: true,
            default: "/"
        }
    },
}
</script>

<style scoped></style>