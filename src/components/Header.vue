<script setup lang="ts">
    import RouterLinkButton from './RouterLinkButton.vue';

    function scrollToTarget(target: string) {
        document.getElementById(target)?.scrollIntoView({behavior: 'smooth', block: 'start', inline: 'nearest'})
    }
</script>

<template>
    <div>
        <header v-bind:style="$route.name === 'landing-page' ? 'justify-content: space-between' : 'justify-content: center'">
            <img @click="$route.name ==='landing-page' ? scrollToTarget('main-title') : $router.push({ name: 'landing-page' })" src="../assets/tabbed-social-logo.svg" width="60"/>
            <nav v-show="$route.name === 'landing-page'">
                <button @click="scrollToTarget('what-desc')">What?</button>
                <button @click="scrollToTarget('features-desc')">Features</button>
                <button @click="scrollToTarget('how-desc')">How it works?</button>
                <RouterLinkButton name="Get started!" target="dashboard"/>
            </nav>
        </header>
    </div>
</template>

<style scoped>  
    header {
        display: flex;
        flex-direction: row;
        align-items: center;
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