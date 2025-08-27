<template>
        <h1>Index</h1>
    <Link href="/hello">Show Page</Link>
    <div>The message is {{ message }}</div>
</template>

<script setup lang="ts">
import { Link } from "@inertiajs/vue3";
// defineProps(['message'])
// specify the type: recommended
defineProps({message: String,})
</script>

<script lang="ts">
import MainLayout from "@/layouts/MainLayout.vue";
export default {
    layout: MainLayout
}
</script>