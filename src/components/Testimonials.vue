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

.card {
  margin-bottom: 24px;
  width: 90%;
  min-width: 424px;
  min-height: 200px; /* lowered height */
  border-radius: 28px;
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
  height: 180px;
  width: 95%;
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

ul{
  list-style: none;
}
</style>