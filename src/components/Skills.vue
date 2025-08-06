<script setup>
import skills from '@/data/Skills.json'

function getImageUrl(filename) {
  // Webpack/Vite will resolve files in /src/assets
  return new URL(`../assets/logos/${filename}`, import.meta.url).href
}
</script>
<template>
  <div class="page-wrapper" id="skills">
    <h1>Skills</h1>
    <p>The skills, tools and technologies I am good at:</p>
    <div class="icons">
      <ul>
       <li v-for="skill in skills" :key="index">
        <div class="logo"> <img :src="getImageUrl(skill.icon)" alt="skill icon"> </div>
        <p>{{ skill.name }}</p>
       </li>
      </ul>
    </div>
  </div>
</template>
<style scoped>
.page-wrapper{
  width: 100%;
  /* min-height: 50%; */
  display: flex;
  flex-direction: column;
  /* place-items: center; */
  text-align: center;
}

/* h1{
  font-weight: 900;
  font-size: 48px;
} */

/* p{
  font-size: 18px;
} */

ul{
  list-style: none;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
}

img{
  height: 100px;
}
</style>