<script setup>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue';
import AboutSection from './components/AboutSection.vue';
import SkillCard from './components/SkillCard.vue';
import ProjectSection from './components/ProjectSection.vue';
import ExperienceTimeline from './components/ExperienceTimeline.vue';
import ContactSection from './components/ContactSection.vue';
</script>

<template>
  <NavBar />
  
  <main>
    <HeroSection/>
    <AboutSection/>
    <SkillCard/>
    <ProjectSection/>
    <ExperienceTimeline/>
    <ContactSection/>
    <div style="height: 1000px;">
    </div>
  </main>
</template>

<style scoped>

</style>