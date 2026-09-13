<script setup lang="ts">
const props = defineProps<{
    text?: string,
}>()
</script>

<template>
    <button>
        <span>{{ text }}</span>
    </button>
</template>

<style scoped>

</style>