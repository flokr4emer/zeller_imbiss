<script setup>
import { RouterLink } from 'vue-router'
import OpeningHoursTableItem from './OpeningHoursTableItem.vue';
import NavItem from './NavItem.vue';
import { headerLinks, footerLinks } from '../js/routerLinks';
</script>

<template>
    <footer class="bd-footer py-4 py-md-5 mt-5 bg-light">
        <div class="container py-4 py-md-5 px-4 px-md-3">
            <div class="row">
                <div class="col-md-6 col-lg-3 mb-3">
                    <RouterLink to="/" class="d-inline-flex align-items-center mb-2 link-dark text-decoration-none">
                        <span class="fs-5">Zeller Imbiss</span>
                    </RouterLink>
                    <ul class="list-unstyled small text-muted">
                        <li class="mb-2">We cook our food with all the love in the world and the best Indian ingredients.
                        </li>
                        <li class="mb-2">Designed and build with &hearts; by
                            <a class="link-dark text-decoration-none" href="https://wwww.gastremo.de">gastremo.de</a>
                        </li>
                        <li class="mb-2">&copy; 2023. Zeller Imbiss.</li>
                    </ul>
                </div>
                <div class="col-sm-12 col-md-6 col-lg-2 offset-lg-1 mb-3">
                    <h5>Contact</h5>
                    <ul class="list-unstyled small text-muted">
                        <li class="mb-2">
                            <a href="tel:078356313870" class="link-dark text-decoration-none">+49 (0) 7835 6313
                                870</a>
                        </li>
                        <li class="mb-2">
                            <a href="mailto:sayhello@zeller-imbiss.de" class="link-dark text-decoration-none">
                                sayhello@zeller-imbiss.de</a>
                        </li>
                        <li class="mb-2">
                            <p>Adress: Steinenfeld 10<br /> 77736 Zell am Harmersbach<br /> Germany</p>
                        </li>
                    </ul>
                </div>
                <div class="col-sm-12 col-md-6 col-lg-2  offset-lg-1 mb-3">
                    <h5>Opening hours</h5>
                    <OpeningHoursTableItem />
                </div>
                <div class="col-sm-12 col-md-6 col-lg-2 offset-lg-1 mb-3">
                    <h5>Links</h5>
                    <ul class="list-unstyled link-dark " v-for="link in headerLinks" :key="link.path">
                        <NavItem :to="link.path" :linkName="link.name" />
                    </ul>
                    <ul class="list-unstyled link-dark " v-for="link in footerLinks" :key="link.path">
                        <NavItem :to="link.path" :linkName="link.name" />
                    </ul>

                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "TheFooter",
}
</script>

<style></style>