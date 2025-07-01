<template>
<Link href="/">Main Page</Link>&nbsp;
<Link href="/hello">Show Page</Link>
<div>This page with time {{ timer }}</div>
<!-- you can add default value inside of slot tag -->
<slot>Default</slot>
</template>

<script setup lang="ts">
import { Link } from "@inertiajs/vue3";
import { ref } from "vue"

// ref create a proxy object
const timer = ref(0)
setInterval(() => {
    timer.value++
}, 1000);
</script>