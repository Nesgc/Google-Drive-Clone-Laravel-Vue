<template>
    <AuthenticatedLayout>

        {{ $page.url }}
    </AuthenticatedLayout>
</template>

<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';

import { Menu, MenuButton, MenuItems, MenuItem } from '@headlessui/vue'
import ResponsiveNavLink from '@/Components/ResponsiveNavLink.vue';
</script>

<style></style>