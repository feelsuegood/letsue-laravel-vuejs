<template>
    <h1>Index {{ counter }}</h1>
</template>

<script setup lang="ts">
import { ref } from "vue";
const counter = ref(0);
setInterval(()=> counter.value++, 1000)
</script>