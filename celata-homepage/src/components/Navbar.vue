<template>
  <nav class="navbar navbar-expand-lg bg-white border-bottom py-3">
    <div class="container">

      <!-- Logo -->
      <a class="navbar-brand d-flex align-items-center" href="#">
        <img :src="logo" alt="Celata Logo" class="navbar-logo" />
      </a>

      <!-- Mobile Toggle -->
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarContent"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Collapsible Content -->
      <div class="collapse navbar-collapse" id="navbarContent">

        <!-- Center Navigation Links -->
        <ul class="navbar-nav mx-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link" href="#">Home</a>
          </li>

          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
            >
              About Us
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#">Company</a></li>
              <li><a class="dropdown-item" href="#">Team</a></li>
            </ul>
          </li>

          <li class="nav-item">
            <a class="nav-link" href="#">Careers</a>
          </li>

          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
            >
              Our Platforms
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#">GeoBizz</a></li>
              <li><a class="dropdown-item" href="#">Sales Force</a></li>
            </ul>
          </li>

          <li class="nav-item">
            <a class="nav-link" href="#">News & Events</a>
          </li>
        </ul>

        <!-- Contact Button -->
        <div class="ms-lg-3 mt-3 mt-lg-0">
          <a class="btn btn-primary px-4 rounded-3 fw-medium" href="#">
            Contact Us
          </a>
        </div>

      </div>
    </div>
  </nav>
</template>

<script setup>
import logo from '../assets/logo.png'
</script>

<style scoped>
.navbar-logo {
  height: 36px;
}

@media (min-width: 992px) {
  .navbar-logo {
    height: 40px;
  }
}
</style>
