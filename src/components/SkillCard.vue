<script setup>
</script>

<template>
  <section id="skills" class="skills">
    <h2 class="section-title">Technical <span>Skill</span></h2>
    
    <div class="skills-grid">
      <div class="skill-card">
        <div class="card-header">
          <h3>Front-End</h3>
        </div>
        <ul class="skill-list">
          <li>Vue.js</li>
          <li>JavaScript</li>
          <li>HTML & CSS</li>
          <li>Java (OOP)</li>
        </ul>
      </div>

      <div class="skill-card">
        <div class="card-header">
          <h3>Back-End</h3>
        </div>
        <ul class="skill-list">
          <li>Spring Boot</li>
          <li>NestJS</li>
          <li>Laravel</li>
        </ul>
      </div>

      <div class="skill-card">
        <div class="card-header">
          <h3>Databases</h3>
        </div>
        <ul class="skill-list">
          <li>MySQL</li>
          <li>MongoDB</li>
          <li>PostgreSQL</li>
        </ul>
      </div>

      <div class="skill-card">
        <div class="card-header">
          <h3>Tools & DevOps</h3>
        </div>
        <ul class="skill-list">
          <li>Docker</li>
          <li>Jenkins & Ansible</li>
          <li>Git Collaboration</li>
          <li>CapCut (Video Editing)</li>
        </ul>
      </div>
    </div>
  </section>
</template>

<style scoped>
.skills {
  padding: 100px 5%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.section-title {
  font-size: 2.5rem;
  margin-bottom: 3rem;
  color: var(--text-primary);
}

.section-title span {
  color: var(--accent-blue);
}

.skills-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
  width: 100%;
  max-width: 1100px;
}

@media (min-width: 600px) {
  .skills-grid {
    grid-template-columns: 1fr 1fr;
  }
}

/* Desktop Layout */
@media (min-width: 1024px) {
  .skills-grid {
    grid-template-columns: repeat(4, 1fr);
  }
}

.skill-card {
  background: var(--card-bg);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.05);
  border-top: 3px solid var(--accent-blue);
  border-radius: 12px;
  padding: 2rem 1.5rem;
  transition: transform 0.3s ease, box-shadow 0.3s ease, border-top-color 0.3s ease;
}

.skill-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 10px 25px rgba(0, 240, 255, 0.15);
  border-top-color: var(--accent-purple);
}

.card-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1.5rem;
  padding-bottom: 1rem;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.card-header h3 {
  font-size: 1.3rem;
  color: var(--text-primary);
}

.skill-list {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 0.8rem;
}

.skill-list li {
  color: var(--text-secondary);
  font-size: 1.05rem;
  display: flex;
  align-items: center;
}

.skill-list li::before {
  content: '';
  display: inline-block;
  width: 8px;
  height: 8px;
  background-color: var(--accent-blue);
  border-radius: 50%;
  margin-right: 12px;
  box-shadow: 0 0 8px var(--accent-blue);
}
</style>