<script setup>
// Standard setup
</script>

<template>
  <section id="experience" class="experience-section">
    <h2 class="section-title">My <span>Journey</span></h2>
    
    <div class="experience-grid">
      
      <div class="experience-card">
        <div class="card-header">
          <span class="date">October 2025 - Present</span>
        </div>
        <h3>Video Editor</h3>
        <h4 class="location">Chrong Baitong / Freelance</h4>
        <p>
          Edited promotional videos using CapCut, enhancing restaurant marketing materials. Gained key skills in visual communication and content presentation.
        </p>
      </div>

      <div class="experience-card">
        <div class="card-header">
          <span class="date">2023 - Present</span>
        </div>
        <h3>Bachelor of Information and Communication Engineering</h3>
        <h4 class="location">Institute of Technology of Cambodia</h4>
        <p>
          Acquired a strong foundation in full-stack web development, software engineering principles, and database management architectures.
        </p>
      </div>

      <div class="experience-card">
        <div class="card-header">
          <span class="date">2024 - 2025</span>
        </div>
        <h3>Restaurant Service Staff</h3>
        <h4 class="location">Chrong Baitong</h4>
        <p>
          Provided customer service, handled orders, and maintained a clean, organized workspace. Developed teamwork and time management skills in a fast-paced environment.
        </p>
      </div>

    </div>
  </section>
</template>

<style scoped>
.experience-section {
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

.experience-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
  width: 100%;
  max-width: 1100px;
}

/* Tablet Layout: 2 columns */
@media (min-width: 768px) {
  .experience-grid {
    grid-template-columns: 1fr 1fr;
  }
}

/* Desktop Layout: 3 columns */
@media (min-width: 1024px) {
  .experience-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

/* --- Card Styles (Matching the Skills section) --- */
.experience-card {
  background: var(--card-bg);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.05);
  border-top: 3px solid var(--accent-blue);
  border-radius: 12px;
  padding: 2rem;
  transition: transform 0.3s ease, box-shadow 0.3s ease, border-top-color 0.3s ease;
  display: flex;
  flex-direction: column;
}

.experience-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 10px 25px rgba(0, 240, 255, 0.15);
  border-top-color: var(--accent-purple);
}

.card-header {
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.date {
  font-family: var(--font-code);
  color: var(--accent-blue);
  font-size: 0.9rem;
  font-weight: bold;
}

.experience-card h3 {
  font-size: 1.3rem;
  color: var(--text-primary);
  margin-bottom: 0.5rem;
  line-height: 1.4;
}

.location {
  font-size: 1rem;
  color: var(--text-secondary);
  font-weight: 500;
  margin-bottom: 1.5rem;
  font-family: var(--font-code);
}

.experience-card p {
  color: var(--text-secondary);
  font-size: 0.95rem;
  line-height: 1.6;
  flex-grow: 1; /* Ensures the text takes up remaining space if card heights differ */
}
</style>