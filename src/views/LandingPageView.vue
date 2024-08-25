<script setup lang="ts">
</script>

<template>
    <main>
        <div id="main-title">
            <div id="title">
                <span style="font-size: 64px;">TabbedSocial</span>
                <span style="font-size: 20px; color: #676767;">Multiple social media in one place</span>
            </div>
            <div id="links">
                <RouterLink to="#">Get started!</RouterLink>
                <RouterLink to="#">What?</RouterLink>
            </div>
        </div>
        <div id="main-description">
            <div id="what-desc" class="container-desc">
                <span>image</span>
                <div class="desc">
                    <span class="title" style="font-size: 24px;">What is TabbedSocial?</span>
                    <span style="font-size: 16px;">Description</span>
                </div>
            </div>
            <div id="features-desc" class="container-desc">
                <div class="desc">
                    <span class="title" style="font-size: 24px;">Features</span>
                </div>
            </div>
            <div id="how-desc" class="container-desc">
                <div class="desc">
                    <span class="title" style="font-size: 24px;">How does it work?</span>
                    <span style="font-size: 16px;">Description</span>
                </div>
                <span>image</span>
                <div class="desc">
                    <span class="title" style="font-size: 24px;">How does it work?</span>
                    <span style="font-size: 16px;">Description</span>
                </div>
            </div>
        </div>
    </main>
</template>

<style scoped>
    main {
        height: 100%;
    }

    #main-title {
        height: 100%;
        padding: 2rem;
        display: flex;
        flex-direction: column;
        gap: 1.5rem;
        align-items: center;
        justify-content: center;
        background-color: var(--color-secondary);
    }
    
    #main-description {
        height: 100%;
    }

    #title {
        font-family: 'Readex Pro', sans-serif;
        font-weight: 600;
        line-height: 40px;
        display: flex;
        flex-direction: column;
        gap: 0.5rem;
        align-items: center;
    }

    #what-desc {
        height: 100%;
        flex-direction: row;
        gap: 1rem;
    }

    #features-desc {
        height: 100%;
    }

    #how-desc {
        height: 100%;
        flex-direction: row;
        gap: 1rem;
    }

    .container-desc {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .desc {
        display: flex;
        flex-direction: column;
        gap: 0.5rem;
        font-family: 'readex pro', sans-serif;
    }

    .desc > .title {
        font-weight: 600;
    }
</style>