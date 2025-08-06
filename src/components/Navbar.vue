<script setup>
</script>
<template>
  <nav>
    <div class="logo"><h1> < MI /> </h1></div>
    <div class="navigation">
      <ul>
        <a href="#">
          <li>Home</li>
        </a>
        <a href="#about">
          <li>About</li>
        </a>
        <a href="#skills">
          <li>Skills</li>
        </a>
        <a href="#experience">
          <li>Experience</li>
        </a>
        <a href="#work">
          <li>Work</li>
        </a>
        <a href="#testimonials">
          <li>Testimonials</li>
        </a>
        <a href="#Blogs">
          <li>Blogs</li>
        </a>
        <a href="#contact">
          <li>Contact</li>
        </a>
        <li> light/dark </li>
        <a href="">
          <li>Download CV</li>
        </a>
      </ul>
    </div>
  </nav>
</template>
<style scoped>
nav{
  height: 100px;
  width: 100vw;
  position: fixed;
  top: 0;
  left: 0;
  /* top: 50%; */
  /* transform: translateY(-50%); */
  /* left: 20px; */
  /* max-width: 100px; */
  z-index: 1000;
  background: #ffffff55;
  backdrop-filter: blur(10px);
  display: flex;
  /* flex-direction: column; */
  place-items: center;
  justify-content: space-between;

}

.logo{
  /* margin-bottom: 50px */
  margin-left: 50px;
}

.logo h1{
  font-weight: 900;
  font-size: 48px;
}

.navigation{
  position: relative;
  /* width: 100%; */
  /* border: 1px solid #fff; */
  margin-right: 50px;
}
.navigation ul{
  width: 50vw;
  position: relative;
  /* border: 1px solid #fff; */
  list-style: none;
  display: flex;
  /* flex-direction: column; */
  place-items: center;
}

a{
  position: relative;
  /* border: 1px solid #fff; */
  width: 100%
}

li{
  position: relative;
  /* border: 1px solid #fff; */
  width: 100%
}
</style>