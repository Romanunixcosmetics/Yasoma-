<script setup>
import { Link } from '@inertiajs/vue3';

</script>

<template>
    <ul class="bb-nav">
        <li class="bb-nav__li">
            <Link :href="route('main')" class="bb-nav__link" :class="{ 'bb-nav__link_active': $page.url === '/' }">Главная</Link>
        </li>
    </ul>
</template>

<style lang="scss" src="./app_navigation.scss"></style>
