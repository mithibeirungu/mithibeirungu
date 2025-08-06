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
        <h1>Curious about me? Here you have it</h1>
        <p>
          I'm a passionate, self-proclaimed designer who specializes in full stack development (Vue.js & Laravel). I am very enthusiastic about bringing the technical and visual aspects of digital products to life. User expereince, pixel perfect design and writing clear, readable, highly performant code matters to me.
        </p>

        <p>
          I begam my journey as a web developer in 2021 and since then, I've continued to grow and evolve as a developer, taking on new challenges and learning the latest technologies along the way. Now in my early 20's, 4 years after starting my web development journey, I'm building cutting-edge web applications using modern technologies such as Vue.js, Laravel, C# and much more.
        </p>

        <p>
          I am very much a progressive thinker and enjoy working on products end to end, from ideation all the way to development.
        </p>

        <p>
          When I'm not in full-on developer mode, you can find me hovering around on twitter or on indie hacker, witnessing the journey of early startups or enjoying some free time. You can follow me on Twitter where I share tech-related bites and build in public or you can follow me on Github.
        </p>

        <p>
          Finally, some quick bits about me.
          <ul>
            <li>Bsc. in Computer Science</li>
            <li>Avid learner</li>
            <li>Full time freelancer</li>
            <li>Aspiring Game developer</li>
          </ul>
          One last thing. I'm available for freelance work, so feel free to reach out and say hello! promise I don't bite
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