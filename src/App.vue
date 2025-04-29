<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <nav>
    <div class="logo-nav">
      <RouterLink to="/">
        <img src="./assets/img/logo1.png" alt="Ben 10 Logo" />
      </RouterLink>
    </div>

    <div class="link-nav">
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/alienigenas">Alienígenas</RouterLink>
      <RouterLink to="/personagens">Personagens</RouterLink>
    </div>
  </nav>

  <RouterView />
</template>

<style scoped>



body {
  background-color: #0c0c0c;
  color: white;
}

/* Navbar */
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 2rem 3rem;
  background-color: #000;
  border-bottom: 3px solid #00ff00;
}

.logo-nav img {
  height: 50px;
}

/* Estilo para os RouterLinks */
.link-nav :deep(a) {
  color: #00ff00;
  text-decoration: none;
  margin-left: 2rem;
  font-size: 1.1rem;
}
</style>
