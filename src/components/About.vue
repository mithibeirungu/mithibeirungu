<script setup></script>
<template>
  <div class="page-wrapper">
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

.image{
  height:414px;
  width: 414px;
  display: flex;
  justify-content: center;
  place-items: center;
  box-shadow: inset 2px 2px 5px #555;
  border-radius: 24px
}

img{
  height: 400px;
  width: 400px;
  border-radius: 16px;
  box-shadow: -1px -1px 5px #555;
}

.text-area{
  width: 60%;
  display: flex;
  place-items: center;
}

.text-area h1{
  font-weight: 900;
  font-size: 48px;
}

.text-area p{
  font-size: 18px;
  margin: 12px;
}
</style>