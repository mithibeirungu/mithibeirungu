<script setup>
import experiences from '@/data/Experiences.json'

function getImageUrl(filename) {
  // Webpack/Vite will resolve files in /src/assets
  return new URL(`../assets/logos/${filename}`, import.meta.url).href
}
</script>
<template>
  <div class="page-wrapper" id="experience">
    <h1>Experience</h1>
    <p>Here is a quick summary of my most recent experiences:</p>
    <div class="experience-cards">
      <ul>
        <li v-for="(experience, index) in experiences" :key="index">
          <div class="card">
            <div class="content">
              <div class="logo"> <img :src="getImageUrl(experience.icon)" alt="Company icon"> </div>
              <div class="contents">
                <h3>{{ experience.role }}</h3>
                <ul>
                  <li v-for="(point, index) in experience.experience" :key="index"> {{ point }}</li>
                </ul>
              </div>
              <div class="dates">
                {{ experience.date }}
              </div>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>
<style scoped>
.page-wrapper{
  position: relative;
  /* border: 1px solid #333; */
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  place-items: center;
}

img{
  height: 100px;
}

ul{
  list-style: none;
}

.experience-cards {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.card {
  position: relative;
  margin-bottom: 24px;
  width: 70%;
  min-width: 400px;
  height: 200px; /* lowered height */
  border-radius: 24px;
  display: flex;
  place-items: center;
  justify-content: center;

  /* Emerald base with gold accents */
  background: linear-gradient(
    135deg,
    #34d399,
    #10b981,
    #059669
  );

  box-shadow:
    0 0 0 3px #d4af37, /* gold border */
    inset 0 0 12px rgba(255, 215, 0, 0.2), /* soft inner shine */
    inset 2px 2px 10px rgba(0, 0, 0, 0.2),
    4px 4px 10px rgba(0, 0, 0, 0.3); /* lift the card */
}

.content {
  position: relative;
  height: calc(100% - 16px);
  width: calc(100% - 16px);
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
  border-radius: 16px;
  padding: 12px;

  background: rgba(255, 255, 255, 0.1); /* subtle overlay for contrast */
  backdrop-filter: blur(4px); /* frosted glass effect */
  border: 1px solid rgba(212, 175, 55, 0.5); /* gold border */
  box-shadow:
    inset 0 0 5px rgba(212, 175, 55, 0.2),
    -1px -1px 5px rgba(255, 255, 255, 0.05),
    2px 2px 6px rgba(0, 0, 0, 0.2);
  color: #f9fefb; /* keep text readable */
  font-weight: 500;
}
</style>