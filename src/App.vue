<template>
  <div class="bg-white text-gray-900 min-h-screen">
    <NavBar />
    <Hero />
    <main>
      <AboutMe />
      <Projects />
      <Experience />
      <Contact />
    </main>

    <footer class="p-4 border-t border-gray-200 bg-black text-center text-[#fce301]">
      &copy; 2024 Mateus Arga. All rights reserved.
    </footer>
  </div>
</template>

<script setup lang="ts">
import Hero from './components/Hero.vue';
import NavBar from './components/NavBar.vue';
import AboutMe from './components/AboutMe.vue';
import Projects from './components/Projects.vue';
import Experience from './components/Experience.vue';
import Contact from './components/Contact.vue';
</script>

<style>
html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  font-family: 'Inter', sans-serif;
}
</style>