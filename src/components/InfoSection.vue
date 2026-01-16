<script setup lang="ts">
import { BContainer, BRow, BCol } from 'bootstrap-vue-next'
</script>

<template>
  <section class="info-section position-relative">
    <BContainer fluid class="h-100">
      <BRow class="h-100 align-items-center g-0">
        <!-- Text Content -->
        <BCol lg="6" class="text-content-col">
          <div class="text-content">
            <h2 class="info-title">Individual & Business Tax Preparation</h2>
            <h3 class="info-subtitle">Servicing Our Community</h3>
            <p class="info-description">
              Our Tax Preparation And Bookkeeping Services Have Been Of Great
              Value To Many Business Owners And Clients Over The Years. We Have
              Decided To Expand Our Territory, Grow And Become Of Value To Our
              Communities. We Are Certified Tax Preparers & Bookkeepers
              Determined To Change The Way You See Taxes And Business Solutions.
            </p>
          </div>
        </BCol>

        <!-- Image Content -->
        <BCol lg="6" class="image-content-col">
          <div class="image-wrapper">
            <img
              src="/assets/WEB/HOME/Banner inferior Individual Business.jpg"
              class="info-image"
              alt="Tax Preparation"
            />
          </div>
        </BCol>
      </BRow>
    </BContainer>
  </section>
</template>

<style scoped>
.info-section {
  background-color: #f8f9fa;
  min-height: 400px;
  overflow: hidden;
}

/* Desktop Layout (lg and up) */
@media (min-width: 992px) {
  .info-section {
    min-height: 500px;
  }

  .text-content-col {
    padding: 4rem 3rem 4rem 5rem;
    background-color: #f8f9fa;
  }

  .image-content-col {
    padding: 0;
    height: 500px;
  }

  .image-wrapper {
    height: 100%;
    width: 100%;
  }

  .info-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: left center;
  }

  .text-content {
    max-width: 600px;
  }

  .info-title {
    font-size: 2.5rem;
    font-weight: 700;
    line-height: 1.2;
    margin-bottom: 1.5rem;
    color: #212529;
  }

  .info-subtitle {
    font-size: 1.75rem;
    font-weight: 600;
    margin-bottom: 2rem;
    color: #212529;
  }

  .info-description {
    font-size: 1rem;
    line-height: 1.6;
    color: #495057;
  }
}

/* Tablet Layout (md to lg) */
@media (min-width: 768px) and (max-width: 991px) {
  .info-section {
    min-height: auto;
  }

  .text-content-col {
    order: 1;
    padding: 3rem 2rem;
    text-align: center;
  }

  .image-content-col {
    order: 2;
    padding: 0;
  }

  .image-wrapper {
    width: 100%;
    height: 400px;
  }

  .info-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
  }

  .text-content {
    max-width: 600px;
    margin: 0 auto;
  }

  .info-title {
    font-size: 2rem;
    font-weight: 700;
    line-height: 1.3;
    margin-bottom: 1.25rem;
    color: #212529;
  }

  .info-subtitle {
    font-size: 1.5rem;
    font-weight: 600;
    margin-bottom: 1.5rem;
    color: #212529;
  }

  .info-description {
    font-size: 0.95rem;
    line-height: 1.6;
    color: #495057;
  }
}

/* Mobile Layout (below md) */
@media (max-width: 767px) {
  .info-section {
    min-height: auto;
  }

  .text-content-col {
    order: 1;
    padding: 2.5rem 1.5rem;
    text-align: center;
  }

  .image-content-col {
    order: 2;
    padding: 0;
  }

  .image-wrapper {
    width: 100%;
    height: 350px;
  }

  .info-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
  }

  .text-content {
    max-width: 100%;
  }

  .info-title {
    font-size: 1.75rem;
    font-weight: 700;
    line-height: 1.3;
    margin-bottom: 1rem;
    color: #212529;
  }

  .info-subtitle {
    font-size: 1.25rem;
    font-weight: 600;
    margin-bottom: 1.25rem;
    color: #212529;
  }

  .info-description {
    font-size: 0.9rem;
    line-height: 1.6;
    color: #495057;
  }
}
</style>
