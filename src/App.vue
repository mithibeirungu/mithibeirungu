<script setup>
// import HelloWorld from './components/HelloWorld.vue'
// import TheWelcome from './components/TheWelcome.vue'
import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Experience from './components/Experience.vue'
</script>

<template>
  <header>
    <Navbar />
  </header>

  <main>
    <Home />
    <About />
    <Skills />
    <Experience />
  </main>
</template>

<style scoped>
header{
  position: sticky;
  top: 0px;
  z-index: 1000;
}

main{
  width: 90vw;
  }
</style>
