<template>
  <Navbar />
  <main>
    <Hero />
    <Products />
    <Clients />
  </main>
  <Footer />
</template>

<script setup>
import Navbar from "./components/Navbar.vue";
import Hero from "./sections/Hero.vue";
import Products from "./sections/Products.vue";
import Clients from "./sections/Clients.vue";
import Footer from "./components/Footer.vue";
</script>
