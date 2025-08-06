<script setup>
import { ref, onMounted } from 'vue'
import skills from '@/data/Skills.json'

const getRandom = (min, max) => Math.random() * (max - min) + min

const icons = ref([])

onMounted(() => {
  icons.value = skills.map((skill, i) => {
    // Randomize animation duration and direction
    const duration = getRandom(12, 22)
    const delay = getRandom(0, duration)
    const startX = getRandom(5, 85)
    const startY = getRandom(5, 85)
    const endX = getRandom(5, 85)
    const endY = getRandom(5, 85)
    return {
      ...skill,
      id: i,
      duration,
      delay,
      startX,
      startY,
      endX,
      endY
    }
  })
})
</script>

<template>
  <div class="icons-bg">
    <div
      v-for="icon in icons"
      :key="icon.id"
      class="icon"
      :style="{
        animation: `floatIcon${icon.id} ${icon.duration}s linear infinite`,
        animationDelay: `${icon.delay}s`
      }"
    >
      <img :src="`/src/assets/logos/${icon.icon}`" :alt="icon.name" />
    </div>
  </div>
</template>

<style scoped>
.icons-bg {
  position: fixed;
  inset: 0;
  z-index: 0;
  pointer-events: none;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
}
.icon {
  position: absolute;
  width: 48px;
  height: 48px;
  opacity: 0.7;
  filter: drop-shadow(0 2px 8px #0002);
}
.icon img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}
/* Keyframes for each icon, generated dynamically */
/* Will be injected below */
</style>

<style>
/* Dynamically generate keyframes for each icon */
/* This will be injected by Vue at runtime */
</style>

<script>
// Inject keyframes for each icon
export default {
  mounted() {
    const styleSheet = document.createElement('style')
    this.$el.appendChild(styleSheet)
    this.$.setupState.icons.forEach(icon => {
      styleSheet.sheet.insertRule(`@keyframes floatIcon${icon.id} {
        0% { top: ${icon.startY}%; left: ${icon.startX}%; }
        50% { top: ${icon.endY}%; left: ${icon.endX}%; }
        100% { top: ${icon.startY}%; left: ${icon.startX}%; }
      }`, styleSheet.sheet.cssRules.length)
    })
  }
}
</script>