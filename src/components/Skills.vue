<script setup>
</script>
<template>
  <div class="page-wrapper">
    <h1>Skills</h1>
    <p>The skills, tools and technologies I am good at:</p>
    <div class="icons">
      <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
        <li>C#</li>
        <li>Vue.js</li>
        <li>Laravel</li>
        <li>PostgreSQL</li>
        <li>Figma</li>
        <li>Git</li>
        <li>Github</li>
      </ul>
    </div>
  </div>
</template>
<style scoped>
.page-wrapper{
  width: 100%;
  min-height: 50%;
  display: flex;
  flex-direction: column;
  /* place-items: center; */
  text-align: center;
}

h1{
  font-weight: 900;
  font-size: 48px;
}

p{
  font-size: 18px;
}

ul{
  list-style: none;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
}
</style>