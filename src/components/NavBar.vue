<script setup>
import { ref } from 'vue';

const menuOpen = ref(false);
function toggleMenu() {
  menuOpen.value = !menuOpen.value;
}
</script>

<template>
  <nav class="navbar">
    <div class="nav-container">
      <a href="#" class="logo">&lt;/DINRASY&gt;</a>
      
      <button class="nav-toggle" @click="toggleMenu" :aria-expanded="menuOpen">
        <span class="bar"></span>
        <span class="bar"></span>
        <span class="bar"></span>
      </button>

      <ul class="nav-links" :class="{ open: menuOpen }">
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 75px;
  /* Uses the CSS variables we set up in main.css */
  background: var(--card-bg); 
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(255, 255, 255, 0.05);
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.3s ease;
}

.nav-container {
  width: 90%;
  max-width: 1200px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-family: var(--font-code);
  font-size: 1.8rem;
  font-weight: bold;
  color: var(--accent-blue);
  text-decoration: none;
  /* Adds a slight neon glow to the logo */
  text-shadow: 0 0 10px rgba(0, 240, 255, 0.4);
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 2.5rem;
}

.nav-links a {
  color: var(--text-primary);
  text-decoration: none;
  font-size: 1rem;
  font-weight: 500;
  transition: color 0.3s ease, text-shadow 0.3s ease;
}

/* Hover effect for the links */
.nav-links a:hover {
  color: var(--accent-blue);
  text-shadow: 0 0 8px var(--accent-blue);
}

/* Mobile nav toggle */
.nav-toggle {
  display: none;
  background: transparent;
  border: none;
  flex-direction: column;
  gap: 6px;
  cursor: pointer;
}
.nav-toggle .bar {
  display: block;
  width: 22px;
  height: 2px;
  background: var(--text-primary);
  border-radius: 2px;
}

@media (max-width: 768px) {
  .nav-links { gap: 1.2rem; }
}

@media (max-width: 430px) {
  .nav-toggle { display: flex; }

  .nav-links {
    display: none;
    position: absolute;
    top: 75px;
    right: 5%;
    background: rgba(15,23,42,0.95);
    backdrop-filter: blur(8px);
    -webkit-backdrop-filter: blur(8px);
    padding: 1rem 1.2rem;
    border-radius: 10px;
    flex-direction: column;
    gap: 1rem;
    box-shadow: 0 8px 30px rgba(2,6,23,0.6);
  }

  .nav-links.open {
    display: flex;
  }

  .nav-links li { white-space: nowrap; }
}
</style>