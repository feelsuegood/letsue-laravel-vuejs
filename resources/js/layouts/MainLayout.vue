<template>
<Link href="/">Main Page</Link>&nbsp;
<Link href="/hello">Show Page</Link>
<!-- you can add default value inside of slot tag -->
<slot>Default</slot>
</template>

<script setup lang="ts">
import { Link } from "@inertiajs/vue3";
</script>