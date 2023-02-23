<script setup>
import {Link, router} from '@inertiajs/vue3';
import AppHeader from "@/Components/Header/AppHeader.vue";
import AppFooter from "@/Components/Footer/AppFooter.vue";

defineProps({
    title: String,
});

const logout = () => {
    router.post(route('logout'));
};
</script>

<template>
    <!-- Page Heading -->
    <header class="sticky top-0 w-full z-40">
        <div class="container">
            <AppHeader/>
        </div>
    </header>

    <!-- Page Content -->
    <main>
        <slot/>
    </main>

    <!-- Page Footer -->
    <footer>
        <div class="container">
            <AppFooter/>
        </div>
    </footer>
</template>
