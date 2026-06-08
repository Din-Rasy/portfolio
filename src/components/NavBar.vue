<script setup>
// We don't need any complex JavaScript here yet!
</script>

<template>
  <nav class="navbar">
    <div class="nav-container">
      <a href="#" class="logo">&lt;/DINRASY&gt;</a>
      
      <ul class="nav-links">
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
</style>