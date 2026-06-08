<script setup>
</script>

<template>
  <section id="about" class="about">
    <h2 class="section-title">About <span>Me</span></h2>
    
    <div class="about-card">
      <div class="about-image-container">
        <img src="/profile.jpg" alt="Din Rasy" class="profile-img" />
        <div class="image-glow"></div>
      </div>
      
      <div class="about-content">
        <h3 class="tagline">Driving Digital Innovation</h3>
        <p>
          I am a fourth-year Information and Communication Engineering student at the Institute of Technology of Cambodia with a strong foundation in full-stack web development.
        </p>
        <p>
          Passionate about building innovative software solutions, I bring strong analytical problem-solving and collaborative skills to the table. I am highly motivated to grow professionally under the guidance of experienced developers and make a meaningful impact in the ever-evolving digital landscape.
        </p>
        
        <div class="quick-facts">
          <div class="fact">
            <span class="label">Location:</span>
            <span class="value">Khan Mean Chey, Phnom Penh</span>
          </div>
          <div class="fact">
            <span class="label">Education:</span>
            <span class="value">Bachelor of Information and Communication Engineering</span>
          </div>
          <div class="fact">
            <span class="label">Languages:</span>
            <span class="value">Khmer, English</span>
          </div>
          <div class="fact">
            <span class="label">Hobbies:</span>
            <span class="value">Learning Frameworks, Coding, Exploring</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.about {
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

.about-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 3rem;
  background: var(--card-bg);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.05);
  border-radius: 20px;
  padding: 3rem;
  max-width: 1000px;
  width: 100%;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
}

@media (min-width: 768px) {
  .about-card {
    flex-direction: row;
    align-items: flex-start;
  }
}

.about-image-container {
  position: relative;
  width: 250px;
  height: 250px;
  flex-shrink: 0;
}

.profile-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 50%;
  position: relative;
  z-index: 2;
  border: 3px solid var(--accent-blue);
}

.image-glow {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  height: 100%;
  background: var(--accent-blue);
  border-radius: 50%;
  filter: blur(30px);
  opacity: 0.3;
  z-index: 1;
  animation: pulse 4s infinite alternate;
}

@keyframes pulse {
  0% { transform: translate(-50%, -50%) scale(1); opacity: 0.3; }
  100% { transform: translate(-50%, -50%) scale(1.1); opacity: 0.5; }
}

.about-content {
  flex: 1;
}

.tagline {
  font-family: var(--font-code);
  color: var(--accent-purple);
  margin-bottom: 1.5rem;
  font-size: 1.2rem;
}

.about-content p {
  color: var(--text-secondary);
  line-height: 1.8;
  margin-bottom: 1.5rem;
  font-size: 1.05rem;
}

.quick-facts {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.5rem;
  margin-top: 2rem;
  padding-top: 2rem;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
}

@media (min-width: 600px) {
  .quick-facts {
    grid-template-columns: 1fr 1fr;
  }
}

.fact {
  display: flex;
  flex-direction: column;
}

.label {
  font-family: var(--font-code);
  color: var(--accent-blue);
  font-size: 0.9rem;
  margin-bottom: 0.3rem;
}

.value {
  color: var(--text-primary);
  font-weight: 500;
}
</style>