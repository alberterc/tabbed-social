<script setup lang="ts">
    import { RouterLink } from 'vue-router';

    defineProps({
        name: String
    })
</script>

<template>
    <RouterLink to="#">{{ name }}</RouterLink>
</template>

<style scoped>
    a {
        color: var(--color-text);
        text-decoration: none;
        transition: 0.3s;
        font-weight: 700;
        background-color: #3F3E5F;
        padding: 0.3rem;
        padding-left: 1.5rem;
        padding-right: 1.5rem;
        border-radius: 8px;
    }

    a:hover {
        background-color: rgba(116, 116, 116, 0.507);
    }
    
    a:active {
        background-color: rgba(116, 116, 116, 0.308);
    }
</style>