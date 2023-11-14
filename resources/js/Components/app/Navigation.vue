<template>
    <nav class="min-w-[200px]">

        <Link class="h-[80px] px-3 flex items-center gap-3" :href="route('myFiles')">
        <ApplicationLogo class="block h-9 w-auto fill-current text-gray-800" />

        GoogleDrive NesGC</Link>

        <div class="px-3">
            <CreateNewDropdown />
            <div class="py-3">
                <NavLink :href="route('myFiles')" :active="$page.url == '/my-files'">My Files</NavLink>
                <NavLink href="/">Shared with Me</NavLink>
                <NavLink href="/">Shared by me</NavLink>
                <NavLink href="/">Trash.</NavLink>

            </div>
        </div>
    </nav>
</template>

<script setup>
import ApplicationLogo from '@/Components/ApplicationLogo.vue';
import CreateNewDropdown from '@/Components/app/CreateNewDropdown.vue';

import { Link } from '@inertiajs/vue3'
import NavLink from '../NavLink.vue';

</script>

<style></style>