<template>
  <section class="clients-section py-5">
    <div class="container">
      <!-- Section Title -->
      <div class="text-center mb-4">
        <h2 class="section-title mb-2">Our Clients</h2>
        <p class="text-muted mb-0 clients-subtext">
          Trusted by industry leaders to deliver intelligent, data-driven solutions.
        </p>
      </div>

      <!-- Logo Grid -->
      <div class="row g-4 justify-content-center mt-4">
        <div
          v-for="client in clients"
          :key="client.name"
          class="col-6 col-md-4"
        >
          <div class="client-tile">
            <img
              :src="client.logo"
              :alt="client.name"
              class="client-logo"
              loading="lazy"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import damro from '../assets/clients/damro.png'
import kpmg from '../assets/clients/kpmg.png'
import leco from '../assets/clients/leco.png'
import nsb from '../assets/clients/nsb.png'
import uniliver from '../assets/clients/uniliver.png'
import worldBank from '../assets/clients/world_bank.png'

const clients = [
  { name: 'Damro', logo: damro },
  { name: 'KPMG', logo: kpmg },
  { name: 'LECO', logo: leco },
  { name: 'NSB', logo: nsb },
  { name: 'Unilever', logo: uniliver },
  { name: 'World Bank', logo: worldBank },
]
</script>

<style scoped>
.clients-section {
  background: #ffffff;
}

.clients-subtext {
  max-width: 680px;
  margin: 0 auto;
}

.client-tile {
  width: 100%;
  aspect-ratio: 1 / 1;
  border-radius: 14px;
  background: #f3f4f6;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.05);

  display: flex;
  align-items: center;
  justify-content: center;

  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.client-tile:hover {
  transform: translateY(-4px);
  box-shadow: 0 14px 32px rgba(0, 0, 0, 0.08);
}

.client-logo {
  max-width: 65%;
  max-height: 50%;
  object-fit: contain;
  transition: transform 0.2s ease;
}

.client-tile:hover .client-logo {
  transform: scale(1.05);
}
</style>
