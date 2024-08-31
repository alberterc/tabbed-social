<script setup lang="ts">
    import RouterLinkButton from './RouterLinkButton.vue';

    function scrollToTarget(target: string) {
        document.getElementById(target)?.scrollIntoView({behavior: 'smooth', block: 'start', inline: 'nearest'})
    }
</script>

<template>
    <div>
        <header>
            <img @click="scrollToTarget('main-title')" src="../assets/tabbed-social-logo.svg" width="60"/>
            <nav>
                <button @click="scrollToTarget('what-desc')">What?</button>
                <button @click="scrollToTarget('features-desc')">Features</button>
                <button @click="scrollToTarget('how-desc')">How it works?</button>
                <RouterLinkButton name="Get started!" />
            </nav>
        </header>
    </div>
</template>

<style scoped>  
    header {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        padding: 1.5rem;
        padding-left: 2rem;
        padding-right: 2rem;
        background: var(--color-primary);
        position: fixed;
        top: 0;
        width: 100%;
    }

    img {
        cursor: pointer;
    }
    
    nav {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 1rem;
    }
</style>