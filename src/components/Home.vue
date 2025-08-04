<script setup>
</script>
<template>
  <div class="page-wrapper">
    <div class="text-area">
      <div class="introduction-text">
        <h1>Hi, I'm Mithibe</h1>
        <p>
          I'm a full stack developer [Vue.js & Laravel] with a focus on creating (and occasionally designing) excpetional digital experiences that are fast, accessible, visually appealing and responsive. Even though I have been creating web application for over 7 years, I still love it as if it was something new.
        </p>
      </div>

      <div class="extras">
        Nairobi, Kenya
        Available for new projects
      </div>

      <div class="socials">
        <ul>
          <li>Github</li>
          <li>Twitter</li>
          <li>Figma</li>
        </ul>
      </div>
    </div>

    <div class="image-area">
      <div class="image">
        <img src="../assets/Mithibe.jpg" alt="I am supposed to be here somewhere">
      </div>
    </div>
  </div>
</template>
<style scoped>
.page-wrapper{
  display: flex;
  height: 100%;
  width: 100%;
}
.text-area{
  height: 100%;
  width: 60%;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
}

.text-area h1{
  font-weight: 900;
  font-size: 48px;
}

.text-area p{
  font-size: 18px;
}

.extras{
  font-size: 18px;
}

.socials ul{
  list-style: none;
  font-size: 18px;
  display: flex;
  justify-content: space-evenly;
}

.image-area{
  height: 100%;
  width: 40%;
  display: flex;
  place-items: center;
  justify-content: center;
  align-items: center;
}

.image{
  /* max-height: 400px; */
  /* max-width: 400px; */
  width: 412px;
  height: 412px;
  box-shadow: inset 2px 2px 5px #555;
  border-radius: 22px;
  display: flex;
  place-items: center;
  justify-content: center;
}

img{
  height: 400px;
  border-radius: 16px;
  box-shadow: -1px -1px 5px #555;
}
</style>