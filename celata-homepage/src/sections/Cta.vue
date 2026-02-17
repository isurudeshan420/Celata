<template>
  <section class="cta-section py-5">
    <div class="container">
      <div class="cta-card text-center">
        <h2 class="cta-title mb-3">
          Ready to transform your operations
        </h2>

        <p class="cta-subtext mb-4">
          See how Celata Tech delivers measurable results for teams across industries.
        </p>

        <div class="d-flex justify-content-center gap-3 flex-wrap">
          <a href="#" class="btn btn-primary px-4 rounded-3">
            Contact Us
          </a>

          <a href="#" class="btn btn-outline-light px-4 rounded-3">
            Learn More
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.cta-section {
  background: #000000;
}

/* Red Card */
.cta-card {
  background:rgb(80, 10, 10);
  border-radius: 16px;
  padding: 60px 24px;
  color: #ffffff;
  box-shadow: 0 20px 50px rgba(0, 0, 0, 0.4);
}

/* Title */
.cta-title {
  font-size: 2rem;
  font-weight: 700;
}

/* Subtext */
.cta-subtext {
  max-width: 600px;
  margin: 0 auto;
  opacity: 0.9;
  line-height: 1.6;
}

/* Desktop Enhancement */
@media (min-width: 992px) {
  .cta-card {
    padding: 80px 60px;
  }

  .cta-title {
    font-size: 3rem;
  }
}
</style>
