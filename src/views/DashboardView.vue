<script setup lang="ts">
    import SocialIcons from '@/components/SocialIcons.vue';
</script>

<template>
    <main>
        <div id="main-dashboard">
            <div id="dashboard-sidebar">
                <SocialIcons name="icon-plus" icon="src/assets/icon-plus.svg" />
            </div>
            <div id="dashboard-content">
                <!-- <iframe src="https://jisho.org/"></iframe> -->
            </div>
        </div>
    </main>
</template>

<style scoped>
    main {
        color: white;
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100%;
    }

    #main-dashboard {
        height: 100%;
        width: 100%;
        display: flex;
        flex-direction: row;
    }

    #dashboard-sidebar {
        height: 100%;
        width: 70px;
        display: grid;
        justify-content: center;
        align-items: center;
    }
    
    #dashboard-content {
        height: 100%;
        width: 100%;
        background-color: var(--color-secondary);
        display: grid;
        align-items: center;
    }

    iframe {
        margin-left: auto;
        margin-right: auto;
        width: 80%;
        height: 80%;
    }
</style>