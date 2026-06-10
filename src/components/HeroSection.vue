<script setup>
</script>

<template>
  <section id="home" class="hero">
    <div class="hero-container">
      <div class="hero-content">
        <p class="greeting">Hi, I'm</p>
        <h1 class="name">DIN RASY</h1>
        <h2 class="role">
          <span class="typing">Full-Stack Web Developer</span>
        </h2>
        <p class="pitch">
          Fourth-year Information and Communication Engineering student passionate about building innovative software solutions and driving digital innovation.
        </p>
        <div class="hero-buttons">
          <a href="#projects" class="btn-primary">View Projects</a>
          <a href="/DIN RASY_CURRICULM VITAE.pdf" download="DIN RASY_CURRICULM VITAE.pdf" class="btn-secondary">
            Download CV
          </a>        
        </div>
      </div>

      <div class="hero-visual">
        <div class="floating-shape">
          <div class="shape-inner">
            <span class="code-symbol">&lt;/&gt;</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding-top: 75px; 
}

.hero-container {
  width: 90%;
  max-width: 1200px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 2rem;
}

.hero-content {
  flex: 1;
  max-width: 600px;
}

.greeting {
  font-family: var(--font-code);
  color: var(--accent-blue);
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
}

.name {
  font-size: 4rem;
  font-weight: 800;
  line-height: 1.1;
  margin-bottom: 1rem;
  color: var(--text-primary);
}

.role {
  font-size: 1.8rem;
  color: var(--text-secondary);
  margin-bottom: 1.5rem;
  font-weight: 500;
}


.typing {
  display: inline-block;
  overflow: hidden;
  white-space: nowrap;
  border-right: .12em solid var(--accent-blue);
  animation: typing 2.5s steps(24, end), blink-caret .75s step-end infinite;
  font-weight: 500;
  vertical-align: bottom;
}

@keyframes typing {
  from { width: 0; }
  to { width: 24ch; }
}

@keyframes blink-caret {
  50% { border-color: transparent; }
}

.pitch {
  font-size: 1.1rem;
  color: var(--text-secondary);
  margin-bottom: 2.5rem;
  line-height: 1.8;
}

.hero-buttons {
  display: flex;
  gap: 1.5rem;
}

.btn-secondary {
  background-color: transparent;
  color: var(--accent-blue);
  padding: 10px 24px;
  border: 1px solid var(--accent-blue);
  border-radius: 8px;
  font-weight: bold;
  text-decoration: none;
  transition: all 0.3s ease;
}

.btn-secondary:hover {
  background-color: rgba(0, 240, 255, 0.1);
  box-shadow: 0 0 15px rgba(0, 240, 255, 0.3);
}

.btn-primary {
  text-decoration: none;
  display: inline-block;
}

.hero-visual {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.floating-shape {
  width: 300px;
  height: 300px;
  background: linear-gradient(135deg, rgba(0, 240, 255, 0.2), rgba(139, 92, 246, 0.2));
  border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
  border: 2px solid rgba(0, 240, 255, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  animation: float 6s ease-in-out infinite, morph 8s ease-in-out infinite;
  box-shadow: 0 0 30px rgba(0, 240, 255, 0.2);
}

.code-symbol {
  font-family: var(--font-code);
  font-size: 4rem;
  font-weight: bold;
  color: var(--accent-blue);
  text-shadow: 0 0 15px var(--accent-blue);
}

@keyframes float {
  0% { transform: translateY(0px); }
  50% { transform: translateY(-20px); }
  100% { transform: translateY(0px); }
}

@keyframes morph {
  0% { border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; }
  50% { border-radius: 70% 30% 30% 70% / 70% 70% 30% 30%; }
  100% { border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; }
}

/* Responsive adjustments for smaller screens (phones, iPhone 17 Pro Max width ~430px) */
@media (max-width: 768px) {
  .hero-container { gap: 1rem; }
  .name { font-size: 3.2rem; }
  .role { font-size: 1.4rem; }
}

@media (max-width: 430px) {
  .hero {
    padding-top: 80px; /* ensure space for fixed navbar */
  }

  .hero-container {
    flex-direction: column;
    align-items: flex-start;
    gap: 1.2rem;
  }

  .hero-content { width: 100%; }

  .name { font-size: 2.6rem; }
  .role { font-size: 1.1rem; }
  .pitch { font-size: 1rem; line-height: 1.5; }

  .hero-buttons { flex-direction: column; width: 100%; }
  .hero-buttons .btn-primary, .hero-buttons .btn-secondary { width: 100%; text-align: center; }

  /* Hide the large visual on small screens to save space */
  .hero-visual { display: none; }
}
</style>