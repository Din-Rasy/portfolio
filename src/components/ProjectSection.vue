<script setup>
</script>

<template>
  <section id="projects" class="projects">
    <h2 class="section-title">Project <span>Experience</span></h2>
    
    <div class="project-grid">
      
      <div class="project-card">
        <div class="project-content">
          <div class="project-header">
            <h3>Jomnus Website ( ជំនួស )</h3>
            <div class="tech-tags">
              <span class="tag">NestJS</span>
              <span class="tag">Next.js</span>
            </div>
          </div>
          <p class="project-desc">
            Micro Task platform connecting users with everyday or personal requests.
          </p>
          <div class="project-links">
            <a href="#" class="link-btn">Live Demo</a>
            <a href="#" class="link-btn outline">GitHub</a>
          </div>
        </div>
      </div>

      <div class="project-card">
        <div class="project-content">
          <div class="project-header">
            <h3>Perfume E-Commerce Website</h3>
            <div class="tech-tags">
              <span class="tag">Vue.js</span>
            </div>
          </div>
          <p class="project-desc">
            Online store with dynamic product display, search functionality, and an integrated shopping cart.
          </p>
          <div class="project-links">
            <a href="https://www.youtube.com/@rasydin-d7p" class="link-btn">Live Demo</a>
            <a href="https://github.com/Perfume-E-commer/Perfume-e-commerce-website" class="link-btn outline">GitHub</a>
          </div>
        </div>
      </div>

      <div class="project-card">
        <div class="project-content">
          <div class="project-header">
            <h3>Enrollment Management System</h3>
            <div class="tech-tags">
              <span class="tag">Spring Boot</span>
            </div>
          </div>
          <p class="project-desc">
            Web-based system designed for student enrollment featuring complete CRUD operations and user authentication.
          </p>
          <div class="project-links">
            <a href="https://www.youtube.com/@rasydin-d7p" class="link-btn">Live Demo</a>
            <a href="https://github.com/Chumdararith-LOU/Project-3-Course-Enrollment-and-Classroom-Scheduling-System" class="link-btn outline">GitHub</a>
          </div>
        </div>
      </div>

    </div>
  </section>
</template>

<style scoped>
.projects {
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

.project-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
  width: 100%;
  max-width: 1100px;
}

@media (min-width: 768px) {
  .project-grid {
    grid-template-columns: 1fr 1fr;
  }
}

@media (min-width: 1024px) {
  .project-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

.project-card {
  background: var(--card-bg);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.05);
  border-radius: 12px;
  overflow: hidden;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  display: flex;
  flex-direction: column;
}

.project-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 15px 30px rgba(0, 240, 255, 0.1);
  border-color: rgba(0, 240, 255, 0.3);
}

.project-content {
  padding: 2rem;
  display: flex;
  flex-direction: column;
  height: 100%;
}

.project-header h3 {
  font-size: 1.4rem;
  color: var(--text-primary);
  margin-bottom: 1rem;
}

.tech-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-bottom: 1rem;
}

.tag {
  background: rgba(139, 92, 246, 0.2);
  color: var(--accent-purple);
  padding: 4px 10px;
  border-radius: 20px;
  font-size: 0.8rem;
  font-family: var(--font-code);
  border: 1px solid rgba(139, 92, 246, 0.3);
}

.project-desc {
  color: var(--text-secondary);
  font-size: 1rem;
  line-height: 1.6;
  margin-bottom: 2rem;
  flex-grow: 1; 
}

.project-links {
  display: flex;
  gap: 1rem;
}

.link-btn {
  text-decoration: none;
  font-size: 0.9rem;
  font-weight: bold;
  padding: 8px 16px;
  border-radius: 6px;
  transition: all 0.3s ease;
  background: var(--accent-blue);
  color: #000;
}

.link-btn:hover {
  box-shadow: 0 0 10px var(--accent-blue);
}

.link-btn.outline {
  background: transparent;
  color: var(--text-primary);
  border: 1px solid rgba(255, 255, 255, 0.2);
}

.link-btn.outline:hover {
  border-color: var(--text-primary);
  box-shadow: none;
  background: rgba(255, 255, 255, 0.05);
}
</style>