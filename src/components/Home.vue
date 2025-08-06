<script setup>
</script>
<template>
  <div class="page-wrapper" id="home">
    <div class="text-area">
      <div class="introduction-text">
        <h1>Hi, I'm Mithibe</h1>
        <h3>Crafting Code, Pixels & Play</h3>
        <p>
          I'm a future focused web developer diving deep into software engineering, UI/UX design and game development. Building clean interfaces, functional systems and immersive expereinces.
        </p>
      </div>

      <div class="call-to-action">
        <ul>
          <li><a href="#work">Explore My Work</a></li>
          <li><a href="#blogs">Read My Blogs</a></li>
          <li><a href="#contacts">Let's Talk</a></li>
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
  margin-bottom: 16px;
}

.text-area p{
  margin-bottom: 64px;
}

/* .extras{
  font-size: 18px;
} */

.socials ul{
  position: absolute;
  bottom: 80px;
  list-style: none;
  /* font-size: 18px; */
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

</style>