<script setup>
</script>

<template>
  <section id="contact" class="contact-section">
    <h2 class="section-title">Let's <span>Collaborate</span></h2>
    <p class="subtitle">Feel free to reach out. I am always open to discussing new projects, creative ideas, or opportunities.</p>
    
    <div class="contact-card">
      <h3>Connect With Me</h3>
      
      <div class="info-list">
        <div class="info-item">
          <span class="icon">📍</span>
          <p>Khan Mean Chey, Phnom Penh</p>
        </div>
        <div class="info-item">
          <span class="icon">📞</span>
          <p>0963020711</p>
        </div>
        <div class="info-item">
          <span class="icon">✉️</span>
          <a href="mailto:rasydin77@gmail.com">rasydin77@gmail.com</a>
        </div>
      </div>

      <div class="social-links">
        <a href="https://www.linkedin.com/in/din-rasy-2511423b1/?skipRedirect=true" class="social-btn">LinkedIn</a>
        <a href="https://github.com/Din-Rasy" class="social-btn">GitHub</a>
        <a href="https://www.youtube.com/@rasydin-d7p" class="social-btn">YouTube</a>
        <a href="https://t.me/Din_Rasy" class="social-btn">Telegram</a>
      </div>
    </div>

    <footer class="footer">
      <p>&copy; 2026 Din Rasy</p>
      <p class="footer-tag">Built with <span class="vue-color">Vue.js</span></p>
    </footer>
  </section>
</template>

<style scoped>
.contact-section {
  padding: 100px 5% 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.section-title {
  font-size: 2.5rem;
  margin-bottom: 0.5rem;
  color: var(--text-primary);
}

.section-title span {
  color: var(--accent-blue);
}

.subtitle {
  color: var(--text-secondary);
  margin-bottom: 4rem;
  text-align: center;
  max-width: 600px;
}

.contact-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  max-width: 600px; 
  background: var(--card-bg);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.05);
  border-radius: 12px;
  padding: 3rem;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
  text-align: center;
  transition: transform 0.3s ease, border-color 0.3s ease;
}

.contact-card:hover {
  transform: translateY(-5px);
  border-color: rgba(0, 240, 255, 0.2);
}

.contact-card h3 {
  font-size: 1.8rem;
  margin-bottom: 2rem;
  color: var(--accent-blue);
}

.info-list {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  margin-bottom: 2.5rem;
  width: 100%;
  align-items: start; 
}

.info-item {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.info-item .icon {
  font-size: 1.2rem;
}

.info-item p, .info-item a {
  color: var(--text-secondary);
  text-decoration: none;
  font-size: 1.1rem;
  transition: color 0.3s ease;
}

.info-item a:hover {
  color: var(--accent-blue);
  text-shadow: 0 0 8px rgba(0, 240, 255, 0.4);
}

.social-links {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
  justify-content: center;
  width: 100%;
  padding-top: 2rem;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
}

.social-btn {
  background: rgba(255, 255, 255, 0.05);
  color: var(--text-primary);
  text-decoration: none;
  padding: 10px 20px;
  border-radius: 8px;
  border: 1px solid rgba(255, 255, 255, 0.1);
  transition: all 0.3s ease;
  font-size: 0.95rem;
  font-weight: 500;
}

.social-btn:hover {
  background: rgba(0, 240, 255, 0.1);
  border-color: var(--accent-blue);
  color: var(--accent-blue);
  box-shadow: 0 0 10px rgba(0, 240, 255, 0.2);
  transform: translateY(-2px);
}

.footer {
  margin-top: 6rem;
  text-align: center;
  border-top: 1px solid rgba(255, 255, 255, 0.05);
  padding-top: 2rem;
  width: 100%;
}

.footer p {
  color: var(--text-secondary);
  font-size: 0.9rem;
  margin-bottom: 0.5rem;
}

.footer-tag {
  font-family: var(--font-code);
  font-size: 0.8rem;
}

.vue-color {
  color: #42b883;
  font-weight: bold;
}
</style>