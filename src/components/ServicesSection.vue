<script setup lang="ts">
import { BContainer, BButton, BRow, BCol } from 'bootstrap-vue-next'
</script>

<template>
  <section class="services-section py-5 text-center bg-light">
    <BContainer>
      <h2 class="mb-5 fw-bold">SERVICES PROVIDED</h2>

      <div
        class="services-layout position-relative d-none d-lg-block"
        style="min-height: 600px"
      >
        <img
          src="/assets/WEB/HOME/Services Provided Women.png"
          class="position-absolute start-50 top-50 translate-middle"
          height="500"
          alt="Services"
        />

        <!-- Icons positioned absolutely (simplified circular layout) -->
        <!-- Top Left -->
        <div class="service-item position-absolute" style="top: 10%; left: 20%">
          <img src="/assets/WEB/HOME/Personal Budgeting.png" width="100" />
          <p class="mt-2 fw-bold">Personal<br />Bookkeeping</p>
        </div>
        <!-- Middle Left -->
        <div class="service-item position-absolute" style="top: 40%; left: 15%">
          <img src="/assets/WEB/HOME/Notary Services.png" width="100" />
          <p class="mt-2 fw-bold">Notary<br />Services</p>
        </div>
        <!-- Bottom Left -->
        <div class="service-item position-absolute" style="top: 70%; left: 20%">
          <img src="/assets/WEB/HOME/Business Solutions.png" width="100" />
          <p class="mt-2 fw-bold">Business<br />Solutions</p>
        </div>

        <!-- Top Right -->
        <div
          class="service-item position-absolute"
          style="top: 10%; right: 20%"
        >
          <img
            src="/assets/WEB/HOME/Individual tax preparation.png"
            width="100"
          />
          <p class="mt-2 fw-bold">Individual Tax<br />Preparation</p>
        </div>
        <!-- Middle Right -->
        <div
          class="service-item position-absolute"
          style="top: 40%; right: 15%"
        >
          <img
            src="/assets/PHONE/HOME/Business Tax Preparation.png"
            width="100"
          />
          <p class="mt-2 fw-bold">Business<br />Tax Preparation</p>
        </div>
        <!-- Bottom Right -->
        <div
          class="service-item position-absolute"
          style="top: 70%; right: 20%"
        >
          <img src="/assets/WEB/HOME/Bookeping Services.png" width="100" />
          <p class="mt-2 fw-bold">Bookkeeping<br />Services</p>
        </div>

        <BButton
          variant="primary"
          size="lg"
          class="rounded-pill position-absolute start-50 translate-middle-x"
          style="bottom: 0"
          >SE HABLA ESPAÑOL</BButton
        >
      </div>

      <!-- Mobile/Tablet Stacked Layout for Services -->
      <div class="d-lg-none">
        <BRow>
          <BCol cols="6" md="4" class="mb-4">
            <img
              src="/assets/WEB/HOME/Personal Budgeting.png"
              class="img-fluid mb-2"
            />
            <p class="fw-bold">Personal Bookkeeping</p>
          </BCol>
          <BCol cols="6" md="4" class="mb-4">
            <img
              src="/assets/WEB/HOME/Notary Services.png"
              class="img-fluid mb-2"
            />
            <p class="fw-bold">Notary Services</p>
          </BCol>
          <BCol cols="6" md="4" class="mb-4">
            <img
              src="/assets/WEB/HOME/Business Solutions.png"
              class="img-fluid mb-2"
            />
            <p class="fw-bold">Business Solutions</p>
          </BCol>
          <BCol cols="6" md="4" class="mb-4">
            <img
              src="/assets/WEB/HOME/Individual tax preparation.png"
              class="img-fluid mb-2"
            />
            <p class="fw-bold">Individual Tax Prep</p>
          </BCol>
          <BCol cols="6" md="4" class="mb-4">
            <img
              src="/assets/PHONE/HOME/Business Tax Preparation.png"
              class="img-fluid mb-2"
            />
            <p class="fw-bold">Business Tax Prep</p>
          </BCol>
          <BCol cols="6" md="4" class="mb-4">
            <img
              src="/assets/WEB/HOME/Bookeping Services.png"
              class="img-fluid mb-2"
            />
            <p class="fw-bold">Bookkeeping</p>
          </BCol>
        </BRow>
        <img
          src="/assets/WEB/HOME/Services Provided Women.png"
          class="img-fluid my-4"
          style="max-height: 400px"
        />
        <div>
          <BButton variant="primary" size="lg" class="rounded-pill"
            >SE HABLA ESPAÑOL</BButton
          >
        </div>
      </div>
    </BContainer>
  </section>
</template>

<style scoped>
.service-item {
  width: 150px;
  text-align: center;
}
</style>
