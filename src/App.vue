<script setup>
import { RouterLink, RouterView } from 'vue-router'
import { ref } from 'vue'

const menuAberto = ref(false)
</script>

<template>
  <header>
    <nav>
      <div class="logo-nav">
        <RouterLink to="/">
          <img src="./assets/img/logo1.png" alt="Ben 10 Logo" />
        </RouterLink>
      </div>

      <button class="menu-toggle" @click="menuAberto = !menuAberto">☰</button>

      <div :class="['link-nav', { aberto: menuAberto }]">
        <RouterLink to="/" @click="menuAberto = false">Home</RouterLink>
        <RouterLink to="/alienigenas" @click="menuAberto = false">Alienígenas</RouterLink>
        <RouterLink to="/personagens" @click="menuAberto = false">Personagens</RouterLink>
      </div>
    </nav>
  </header>

  <main>
    <RouterView />
  </main>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: #0c0c0c;
  color: white;
  font-family: sans-serif;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: #000;
  border-bottom: 3px solid #00ff00;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.logo-nav img {
  height: 50px;
}

.link-nav {
  display: flex;
  gap: 2rem;
}

.link-nav a {
  color: #00ff00;
  text-decoration: none;
  font-size: 1.1rem;
}

.menu-toggle {
  display: none;
  font-size: 2rem;
  color: #00ff00;
  background: none;
  border: none;
  cursor: pointer;
}

@media (max-width: 1200px) {
  .link-nav a {
    font-size: 1rem;
  }
}

@media (max-width: 800px) {
  .menu-toggle {
    display: block;
  }

  .link-nav {
    position: absolute;
    top: 100%;
    right: 0;
    background-color: #000;
    flex-direction: column;
    align-items: center;
    width: 100%;
    padding: 1rem 0;
    display: none;
  }

  .link-nav.aberto {
    display: flex;
  }

  .link-nav a {
    padding: 0.5rem 0;
    font-size: 1.2rem;
  }
}

@media (max-width: 400px) {
  .logo-nav img {
    height: 40px;
  }

  .menu-toggle {
    font-size: 1.8rem;
  }

  .link-nav a {
    font-size: 1rem;
  }
}

@media (max-width: 270px) {
  nav {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.5rem;
  }

  .link-nav {
    align-items: flex-start;
  }

  .logo-nav img {
    height: 30px;
  }

  .menu-toggle {
    font-size: 1.5rem;
  }

  .link-nav a {
    font-size: 0.9rem;
  }
}
</style>
