<script setup>
import experiences from '@/data/Experiences.json'

</script>
<template>
  <div class="page-wrapper" id="testimonials">
    <h1>Testimonials</h1>
    <p>Nice things people have said about my work:</p>
    <div class="experience-cards">
      <ul>
        <li v-for="(experience, index) in experiences" :key="index">
          <div class="card">
            <div class="content">
              <div class="logo">{{experience.icon}}</div>
              <contet> {{ experience.experience}}</contet>
              <dates>{{ experience.date }}</dates>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>
<style scoped>
.page-wrapper{
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  place-items: center;
}

.card{
  width: 60%;
  min-width: 424px;
  min-height: 224px;
  box-shadow: inset 2px 2px 5px #555;
  border-radius: 28px;
  display: flex;
  place-items: center;
  justify-content: center;
}
.content{
  height: 200px;
  width: 400px;
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
  border: 1px solid #000;
  box-shadow: -1px -1px 5px #555;
  padding: 6px;
  border-radius: 16px;
}

ul{
  list-style: none;
}
</style>