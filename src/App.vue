<template>
  <header>
    <Navbar />
  </header>

  <!-- Animated icons background -->
  <SkillIconsBackground />

  <!-- Glass layer -->
  <div class="glass-layer"></div>

  <main>
    <Home />
    <About />
    <Skills />
    <Experience />
    <Work />
    <Testimonials />
    <Contact />
  </main>
</template>

<script setup>
import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Experience from './components/Experience.vue'
import Work from './components/Work.vue'
import Testimonials from './components/Testimonials.vue'
import Contact from './components/Contact.vue'
import SkillIconsBackground from './components/SkillIconsBackground.vue'
</script>

<style scoped>
header{
  position: sticky;
  top: 0px;
  z-index: 1000;
}

main{
  width: 90vw;
  position: relative;
  z-index: 2;
}

/* Glass layer styles */
.glass-layer {
  position: fixed;
  inset: 0;
  z-index: 1;
  pointer-events: none;
  width: 100vw;
  height: 100vh;
  background: rgba(255,255,255,0.12);
  backdrop-filter: blur(12px) brightness(1.1);
  border-radius: 0;
}
</style>
