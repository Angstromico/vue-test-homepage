<script setup lang="ts">
import { BContainer, BRow, BCol, BCard, BButton } from 'bootstrap-vue-next'
</script>

<template>
  <section class="testimonials-section py-5 bg-primary text-white">
    <BContainer>
      <h2 class="text-center mb-5">TESTIMONIALS</h2>
      <BRow>
        <BCol md="4" class="mb-4" v-for="i in 3" :key="i">
          <BCard class="text-center h-100 text-dark">
            <img
              src="/assets/WEB/HOME/Testimonials Picture.png"
              class="rounded-circle mb-3"
              width="80"
            />
            <h5 class="fw-bold">Clara Smith</h5>
            <p class="text-muted small">CEO - Any Company</p>
            <hr />
            <p class="card-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
            <BButton variant="primary" size="sm" class="rounded-pill mt-3"
              >Read More</BButton
            >
          </BCard>
        </BCol>
      </BRow>
    </BContainer>
  </section>
</template>

<style scoped>
/* Custom Overrides for Primary Color if needed */
.bg-primary {
  background-color: #0d6efd !important; /* Adjust to match image blue */
}
</style>
