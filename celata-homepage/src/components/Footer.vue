<template>
  <footer class="footer-wrap text-white">
    <div class="container py-5">
      <!-- Top Grid -->
      <div class="row g-4">

        <!-- Brand + Description -->
        <div class="col-12 col-lg-4">
          <div class="d-flex align-items-center gap-2 mb-3">
            <img :src="logo" alt="Celata Logo" class="footer-logo" />
          </div>

          <p class="footer-desc mb-0">
            Delivering intelligent geospatial and AI-driven solutions that empower
            businesses to make smarter, data-backed decisions.
          </p>
        </div>

        <!-- Products -->
        <div class="col-12 col-lg-2">
          <h6 class="footer-title">Products</h6>
          <ul class="footer-links">
            <li><a href="#">Geobizz</a></li>
            <li><a href="#">Sales Force</a></li>
            <li><a href="#">Pricing</a></li>
            <li><a href="#">Documentation</a></li>
            <li><a href="#">API Reference</a></li>
          </ul>
        </div>

        <!-- Company -->
        <div class="col-12 col-lg-2">
          <h6 class="footer-title">Company</h6>
          <ul class="footer-links">
            <li><a href="#">About us</a></li>
            <li><a href="#">Blog</a></li>
            <li><a href="#">Careers</a></li>
            <li><a href="#">Contact</a></li>
            <li><a href="#">Support</a></li>
          </ul>
        </div>

        <!-- Follow Us -->
        <div class="col-12 col-lg-4">
          <h6 class="footer-title">Follow us</h6>
          <ul class="footer-social">
            <li><a href="#"><span class="icon">f</span> Facebook</a></li>
            <li><a href="#"><span class="icon">◎</span> Instagram</a></li>
            <li><a href="#"><span class="icon">x</span> X</a></li>
            <li><a href="#"><span class="icon">in</span> LinkedIn</a></li>
            <li><a href="#"><span class="icon">▶</span> YouTube</a></li>
          </ul>
        </div>

      </div>

      <!-- Divider -->
      <hr class="footer-divider my-4" />

      <!-- Bottom Bar -->
      <div
        class="d-flex flex-column flex-lg-row align-items-start align-items-lg-center justify-content-between gap-3"
      >
        <div class="footer-copy">
          © 2025 Celata Tech. All rights reserved.
        </div>

        <div class="footer-legal d-flex flex-column flex-sm-row gap-2 gap-sm-4">
          <a href="#">Privacy Policy</a>
          <a href="#">Terms of service</a>
          <a href="#">Cookie settings</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
import logo from '../assets/logo.png'
</script>

<style scoped>
.footer-wrap {
  background: #000;
}

.footer-logo {
  height: 28px;
}

.footer-desc {
  max-width: 360px;
  color: rgba(255, 255, 255, 0.75);
  line-height: 1.6;
  font-size: 0.95rem;
}

.footer-title {
  font-weight: 600;
  margin-bottom: 12px;
}

.footer-links,
.footer-social {
  list-style: none;
  padding: 0;
  margin: 0;
  display: grid;
  gap: 10px;
}

.footer-links a,
.footer-social a,
.footer-legal a {
  color: rgba(255, 255, 255, 0.78);
  text-decoration: none;
  font-size: 0.92rem;
}

.footer-links a:hover,
.footer-social a:hover,
.footer-legal a:hover {
  color: #fff;
  text-decoration: underline;
}

.footer-social a {
  display: flex;
  align-items: center;
  gap: 10px;
}

.icon {
  width: 22px;
  height: 22px;
  border-radius: 6px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: rgba(255, 255, 255, 0.08);
  font-size: 0.75rem;
}

.footer-divider {
  border-color: rgba(255, 255, 255, 0.12);
}

.footer-copy {
  color: rgba(255, 255, 255, 0.65);
  font-size: 0.9rem;
}

.footer-legal a {
  color: rgba(255, 255, 255, 0.65);
  font-size: 0.9rem;
}

/* Slight spacing improvement for mobile */
@media (max-width: 991.98px) {
  .footer-title {
    margin-top: 18px;
  }
}
</style>
