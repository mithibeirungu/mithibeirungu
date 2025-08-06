<script setup></script>
<template>
  <div class="page-wrapper" id="about">
    <div class="image-area">
      <div class="image">
        <img src="../assets/Mithibe2.jpg" alt="I am also somewhere around here">
      </div>
    </div>

    <div class="text-area">
      <div class="text-content">
        <h1>Who I am:</h1>
        <p>
          I'm a self-driven creative and problem solver based in Kenya. Right now, I work with HTML, CSS and JavaScript to build responsive, modern websites. But that's just the beginning.
        </p>
        <p>
          I'm Currently learning Vue and Laravel to level up my web development workflow and I'm stepping into the world of software engineering with C#, especially for game development. I also design interfaces using Figma with a strong eye for detail and userbility.
        </p>

        <h3>What Drives Me:</h3>
        <p>
          I'm obsessed with building things, from usable UIs to scalable backends to immersive games. My goal is to become a full-stack builder who can take a product from idea to launch, both visually and functionally.
        </p>
      </div>
    </div>
  </div>
</template>
<style scoped>
.page-wrapper{
  height: 100%;
  width: 100%;
  display: flex;
}

.image-area{
  width: 40%;
  display: flex;
  place-items: center;
  justify-content: center;
}

.image {
  height: 424px;
  width: 424px;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 24px;

  /* Emerald gradient background to mimic shine */
  background: linear-gradient(
    145deg,
    #34d399,
    #10b981,
    #059669
  );

  /* Gold outer border + inner glow */
  box-shadow:
    0 0 0 4px #d4af37,           /* gold outer border */
    inset 0 0 15px rgba(212, 175, 55, 0.5), /* gold inner glow */
    inset -4px -4px 10px rgba(0, 0, 0, 0.2), /* top-left inner bevel */
    inset 4px 4px 10px rgba(255, 255, 255, 0.1); /* bottom-right light */
}

img {
  height: 400px;
  width: 400px;
  border-radius: 16px;

  /* Subtle inset feel with gemstone-like shadow */
  box-shadow:
    0 0 20px rgba(16, 185, 129, 0.4),
    -2px -2px 5px rgba(255, 255, 255, 0.1),
    2px 2px 8px rgba(0, 0, 0, 0.3);

  object-fit: cover;
}


.text-area{
  width: 60%;
  display: flex;
  place-items: center;
}

.text-area h1{
  font-weight: 900;
}

.text-area p{
  margin: 12px;
}

ul{
  display: grid;
  grid-template-columns: 1fr 1fr;
}
</style>