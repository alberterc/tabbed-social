<script setup lang="ts">
    defineProps({
        name: String,
        icon: String
    })
</script>

<template>
    <div class="social-icons-container">
        <img :src=icon :alt=name width="30px" />
    </div>
</template>

<style scoped>
    .social-icons-container {
        background-color: #43254D;
        border-radius: 16px;
        height: 56px;
        width: 56px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .social-icons-container:hover {
        background-color: #ffffff3a;
    }

    .social-icons-container:active {
        background-color: #ffffff56;
    }
</style>