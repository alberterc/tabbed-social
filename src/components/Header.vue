<template>
    <div>
      <header>
        <img src="../assets/tabbed-social-logo.svg" width="60"/>
        <nav>
            <RouterLink to="/features">Features</RouterLink>
            <RouterLink to="/what">What?</RouterLink>
            <RouterLink to="/howitworks">How it works?</RouterLink>
            <RouterLink to="/dashboard">Get started!</RouterLink>
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
  
  nav {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 1rem;
  }

  a {
    color: var(--color-text);
    text-decoration: none;
    transition: 0.4s;
  }

  a:hover {
    background-color: rgba(255, 255, 255, 0.445);
  }
</style>