<template>
  <Navbar />
  <main>
    <Hero />
    <Products />
    <Clients />
    <Cta />
  </main>
  <Footer />
</template>

<script setup>
import Navbar from "./components/Navbar.vue";
import Hero from "./sections/Hero.vue";
import Products from "./sections/Products.vue";
import Clients from "./sections/Clients.vue";
import Cta from "./sections/Cta.vue";
import Footer from "./components/Footer.vue";
</script>
