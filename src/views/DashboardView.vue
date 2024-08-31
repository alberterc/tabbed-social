<template>
    <main>
        <div id="main-dashboard">
            <div id="dashboard-sidebar">

            </div>
            <div id="dashboard-content">
                
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
    }
    
    #dashboard-content {
        height: 100%;
        width: 100%;
        background-color: var(--color-secondary);
    }
</style>