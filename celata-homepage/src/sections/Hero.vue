<template>
  <section
    class="hero-section d-flex align-items-center text-white"
    :style="{
      backgroundImage: `
        linear-gradient(
          rgba(0, 0, 0, 0.4),
          rgba(0, 0, 0, 0.4)
        ),
        url(${heroBg})
      `
    }"
  >
    <div class="container text-center">
      <h1 class="hero-title mb-4">
        Positioning You Globally
      </h1>

      <p class="hero-subtext mb-5">
        Celata Tech delivers cutting-edge geographical intelligence and AI-driven solutions,
        transforming spatial data into meaningful insights for smarter business decisions.
      </p>

      <div class="d-flex justify-content-center gap-3 flex-wrap">
        <a class="btn btn-primary px-4 py-2 rounded-3 fw-medium">
          Contact Us
        </a>

        <a class="btn btn-outline-light px-4 py-2 rounded-3 fw-medium">
          Learn More
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
import heroBg from '../assets/hero-bg.png'
</script>

<style scoped>
.hero-section {
  min-height: 95vh;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

.hero-title {
  font-weight: 700;
  letter-spacing: -1.2px;
}

.hero-subtext {
  max-width: 720px;
  margin: 0 auto;
  font-size: 1rem;
  line-height: 1.6;
  opacity: 0.95;
}

@media (min-width: 992px) {
  .hero-title {
    font-size: 4rem;
  }


  .hero-subtext {
    font-size: 1.15rem;
  }
}
</style>
