<template>
  <section class="products-section py-5">
    <div class="container">
      <!-- Section Title -->
      <div class="text-center mb-5">
        <h2 class="section-title text-white mb-2">Our Products</h2>
        <p class="text-white-50 mb-0">
          Cloud-based location intelligence and mobile engagement in one platform
        </p>
      </div>

      <div class="row g-4">
        <!-- GeoBizz -->
        <div class="col-12 col-lg-6">
          <article
            class="product-card"
            :style="{
              backgroundImage: `
                linear-gradient(
                  rgba(0,0,0,0.4),
                  rgba(0,0,0,0.4)
                ),
                url(${geoBg})
              `
            }"
          >
            <div class="product-content">
              <h3 class="product-title">Geobizz</h3>

              <p class="product-desc">
                GeoBizz is a cloud-based location intelligence platform that
                transforms spatial data into actionable insights—helping businesses
                analyze geographic patterns, track trends, and make smarter
                data-driven decisions.
              </p>

              <a
                href="#"
                class="btn btn-outline-light btn-sm rounded-3 px-4 mt-auto align-self-start"
              >
                Learn More
              </a>
            </div>
          </article>
        </div>

        <!-- SFA -->
        <div class="col-12 col-lg-6">
          <article
            class="product-card"
            :style="{
              backgroundImage: `
                linear-gradient(
                  rgba(0,0,0,0.4),
                  rgba(0,0,0,0.4)
                ),
                url(${sfaBg})
              `
            }"
          >
            <div class="product-content">
              <h3 class="product-title">
                AI-Powered Sales Force Automation
              </h3>

              <p class="product-desc">
                Revolutionize field sales with intelligent route optimization,
                automated reporting, and real-time performance insights that
                drive accountability and growth.
              </p>

              <a
                href="#"
                class="btn btn-outline-light btn-sm rounded-3 px-4 mt-auto align-self-start"
              >
                Learn More
              </a>
            </div>
          </article>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import geoBg from '../assets/geobizz-card.png'
import sfaBg from '../assets/sfa-card.png'
</script>

<style scoped>
.products-section {
  background: #0b0f17;
}

.product-card {
  position: relative;
  display: flex;
  flex-direction: column;
  border-radius: 16px;
  overflow: hidden;
  min-height: 360px;
  background-size: cover;
  background-position: center;
  box-shadow: 0 18px 45px rgba(0, 0, 0, 0.4);
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.product-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 25px 60px rgba(0, 0, 0, 0.5);
}

.product-content {
  flex: 1;
  padding: 28px;
  display: flex;
  flex-direction: column;
  gap: 14px;
  color: #ffffff;
}

.product-title {
  font-size: 2rem;
  font-weight: 700;
  margin: 0;
  color: #ffffff;
}

.product-desc {
  margin: 0;
  max-width: 450px;
  line-height: 1.6;
  color: rgba(255, 255, 255, 0.9);
}

@media (min-width: 992px) {
  .product-card {
    min-height: 400px;
  }

  .product-title {
    font-size: 2.2rem;
  }
}
</style>
