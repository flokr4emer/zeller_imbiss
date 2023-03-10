<script setup>
import { RouterLink } from 'vue-router'
import NavItem from './NavItem.vue'
import NavTogglerItem from './NavTogglerItem.vue'
import { headerLinks } from '../js/routerLinks.js'
</script >

<template>
    <nav class="navbar navbar-expand-lg bg-light">
        <div class="container-fluid">
            <RouterLink to="/" class="navbar-brand">{{ websideName }}</RouterLink>
            <NavTogglerItem />
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <NavItem :to="link.path" :linkName="link.name" v-for="link in headerLinks" :key="link.path" />
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: "TheHeaderNavigation",
    data() {
        return {
            websideName: "Zeller Imbiss",
        };
    },
}
</script>

<style scoped></style>