<template>
    <div>
      <footer>
        <img src="../assets/tabbed-social-logo.svg" width="40"/>
        <span>&copy; 2024 TabbedSocial</span>
      </footer>
    </div>
</template>

<style scoped>
  footer {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 0.1rem;
    padding: 0.5rem;
    padding-left: 2rem;
    padding-right: 2rem;
    background: var(--color-primary);
    position: fixed;
    bottom: 0;
    width: 100%;
    border-top: solid 1px #535353;
  }

  span {
    font-size: 12px;
  }
</style>