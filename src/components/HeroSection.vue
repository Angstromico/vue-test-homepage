<script setup lang="ts">
import { BContainer, BRow, BCol, BButton } from 'bootstrap-vue-next'
</script>

<template>
  <div class="hero-section position-relative text-white mt-5 pt-4">
    <img
      src="/assets/WEB/HOME/Banner principal 1.jpg"
      class="img-fluid w-100 hero-img"
      alt="Banner"
    />
    <div
      class="hero-overlay position-absolute top-0 start-0 w-100 h-100 d-flex align-items-center"
    >
      <BContainer>
        <BRow>
          <BCol md="6" offset-md="6" class="text-end pe-5">
            <h1 class="display-4 fw-bold">INDIVIDUAL TAX<br />PREPARATION</h1>
            <p class="fs-4 fst-italic">You Can Count On...</p>
            <BButton variant="primary" class="rounded-pill mt-3 px-4"
              >Learn More</BButton
            >
          </BCol>
        </BRow>
      </BContainer>
    </div>

    <!-- CTA Cards (overlapping hero slightly) -->
    <div class="cta-cards-container">
      <BContainer>
        <BRow class="g-0">
          <BCol md="4">
            <div
              class="cta-card bg-primary p-4 text-center text-white border-end border-light"
            >
              <img
                src="/assets/WEB/HOME/Individual Tax Preparation Blanco.svg"
                height="50"
                class="mb-3"
              />
              <h5>Individual tax preparation</h5>
            </div>
          </BCol>
          <BCol md="4">
            <div
              class="cta-card bg-primary p-4 text-center text-white border-end border-light"
            >
              <img
                src="/assets/WEB/HOME/Bookepping Blanco.svg"
                height="50"
                class="mb-3"
              />
              <h5>Bookkeeping</h5>
            </div>
          </BCol>
          <BCol md="4">
            <div class="cta-card bg-primary p-4 text-center text-white">
              <img
                src="/assets/WEB/HOME/Business Tax Preparation Blanco.svg"
                height="50"
                class="mb-3"
              />
              <h5>Business tax preparation</h5>
            </div>
          </BCol>
        </BRow>
      </BContainer>
    </div>
  </div>
</template>

<style scoped>
.hero-section {
  overflow: hidden;
}
.hero-img {
  object-fit: cover;
  min-height: 500px; /* Ensure height on mobile */
}
.cta-card {
  height: 100%;
  transition: transform 0.2s;
}
.cta-card:hover {
  transform: translateY(-5px);
}

@media (max-width: 991px) {
  .hero-overlay {
    background: rgba(
      0,
      0,
      0,
      0.4
    ); /* Darken overly on mobile for readability */
  }
}
</style>
