<script setup>
// you can add theme toggling or logic here if needed
</script>

<template>
  <nav class="navbar">
    <div class="logo">MI</div>
    <ul class="nav-links">
      <li><a href="#">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#experience">Experience</a></li>
      <li><a href="#work">Work</a></li>
      <li><a href="#testimonials">Testimonials</a></li>
      <li><a href="#blogs">Blogs</a></li>
      <li><a href="#contact">Contact</a></li>
      <li><button class="theme-toggle">Light/Dark</button></li>
      <li><a class="download-btn" href="#">Download CV</a></li>
    </ul>
  </nav>
</template>

<style scoped>
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  height: 80px;
  width: 100%;
  padding: 0 2rem;
  background: rgba(255, 255, 255, 0.7);
  backdrop-filter: blur(10px);
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  z-index: 1000;

  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  font-size: 2rem;
  font-weight: 800;
  color: #047857; /* emerald green */
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
  align-items: center;
}

.nav-links li {
  position: relative;
}

.nav-links a {
  text-decoration: none;
  color: #1f2937;
  font-weight: 500;
  padding: 8px 12px;
  border-radius: 8px;
  transition: all 0.3s ease;
}

.nav-links a:hover {
  background: #d1fae5;
  color: #065f46;
}

.theme-toggle {
  background: transparent;
  border: 1px solid #d1d5db;
  padding: 6px 10px;
  border-radius: 8px;
  cursor: pointer;
  font-size: 0.9rem;
}

.theme-toggle:hover {
  background: #f3f4f6;
}

.download-btn {
  background: linear-gradient(to right, #047857, #10b981);
  color: white;
  padding: 8px 14px;
  border-radius: 10px;
  font-weight: 600;
  transition: 0.3s ease;
}

.download-btn:hover {
  background: linear-gradient(to right, #065f46, #059669);
}
</style>
