<script setup lang="ts">
    import RouterLinkButton from '@/components/RouterLinkButton.vue';
    import Card from '@/components/Card.vue';

    const features = [
        {
            title: 'Availability',
            desc: 'There are multiple platforms which are available, such as Instagram, X, WhatsApp, and Telegram. More platforms may be added in the future.'
        },
        {
            title: 'Privacy',
            desc: 'TabbedSocial does not store any account information. Instead, it uses the cookies from the social media platforms itself if available.'
        },
        {
            title: 'No Account',
            desc: 'Accounts are not needed. TabbedSocial only provides a dashboard to open multiple social media platforms.'
        },
        {
            title: 'Seamless Switch',
            desc: 'Switch and open social media platforms seamlessly.'
        },
    ]

    const loremIpsumStr = 'Lorem ipsum dolor sit amet, consectetur adispicing elit. Ut aliquet odio at tortor eleifend, quis imperdiet nisi suscipit. Sed in fringilla metus. Nunc nec condimentum mi. Donec dictum solliciudin efficitur. Integer imperdiet feugiat interdum. Sed facilisis felis vel lorem blandit, vel varius sapien scelerisque. Aliquam gravida ultrices dui, non lobortis velit consequat non. Sed ultrices justo nec commodo interdum. Sed quis fringilla erat. Duis id magna lorem.'
</script>

<template>
    <main>
        <div id="main-title">
            <div id="title">
                <span style="font-size: 64px;">TabbedSocial</span>
                <span style="font-size: 20px; color: #676767;">Multiple social media in one place</span>
            </div>
            <div id="links">
                <RouterLinkButton name="Get started!" />
            </div>
        </div>
        <div id="main-description">
            <div id="what-desc" class="container-desc">
                <div class="image-placeholder"></div>
                <div class="desc">
                    <span class="desc-title" style="font-size: 24px;">What is TabbedSocial?</span>
                    <span style="font-size: 16px;">{{ loremIpsumStr }}</span>
                </div>
            </div>
            <div id="features-desc" class="container-desc">
                <span class="desc-title" style="font-size: 24px;">Features</span>
                <div class="cards-container">
                    <div v-for='feature in features' :key='feature.title'>
                        <Card :title='feature.title' :desc='feature.desc'/>
                    </div>
                </div>
            </div>
            <div id="how-desc" class="container-desc">
                <div class="desc" style="width: 360px;">
                    <span class="desc-title" style="font-size: 24px;">How does it work?</span>
                    <span style="font-size: 16px;">{{ loremIpsumStr }}</span>
                </div>
                <div class="image-placeholder"></div>
                <div class="desc" style="width: 360px; text-align: right;">
                    <span class="desc-title" style="font-size: 24px;">How does it work?</span>
                    <span style="font-size: 16px;">{{ loremIpsumStr }}</span>
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
        font-weight: 300;
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
        gap: 2rem;
    }

    #features-desc {
        height: 100%;
        flex-direction: column;
        gap: 2rem;
    }

    #how-desc {
        height: 100%;
        flex-direction: row;
        gap: 2rem;
        padding: 4rem;
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
        width: 768px;
    }

    .desc-title {
        font-weight: 600;
    }

    .cards-container {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 1rem;
    }

    .image-placeholder {
        width: 350px;
        height: 450px;
        border-radius: 16px;
        background-color: rgba(255, 255, 255, 0.158);
    }
</style>