<script setup lang="ts">
    defineProps({
        title: String,
        desc: String
    })
</script>

<template>
    <div class="card">
        <span class="card-title">{{ title }}</span>
        <span class="card-desc">{{ desc }}</span>
    </div>
</template>

<style scoped>
    .card {
        display: flex;
        flex-direction: column;
        gap: 0.5rem;
        padding-left: 18px;
        padding-right: 18px;
        padding-top: 16px;
        padding-bottom: 16px;
        border: solid 1px #535353;
        border-radius: 16px;
        width: 377px;
        height: 178px;
    }

    .card-title {
        font-weight: 700;
        font-size: 20px;
    }

    .card-desc {
        font-size: 16px;
        font-weight: 300;
    }
</style>