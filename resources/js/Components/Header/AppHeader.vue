<script setup>
import { Link } from '@inertiajs/vue3';
import AppLogo from "@/Components/Logo/AppLogo.vue";
import AppNavigation from "@/Components/Navigation/AppNavigation.vue";
</script>

<template>
    <div class="bb-header">
        <!-- Header Logo -->
        <div class="bb-header__logo items-center">
            <Link :href="'/'">
                <AppLogo/>
            </Link>
        </div>

        <!-- Header Navigation -->
        <nav class="bb-header__nav">
            <AppNavigation/>
        </nav>

        <!-- Header Actions -->
        <div class="bb-header__actions">
            <Link :href="route('login')">
                Login
            </Link>
        </div>
    </div>
</template>

<style lang="scss" src="./app_header.scss"></style>
