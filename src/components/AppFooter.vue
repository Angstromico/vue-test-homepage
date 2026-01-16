<script setup lang="ts">
import { BContainer, BButton } from 'bootstrap-vue-next'
</script>

<template>
  <footer class="footer py-5 text-center">
    <BContainer>
      <BButton variant="primary" size="lg" class="rounded-pill mb-4 px-5"
        >BOOK TODAY</BButton
      >
      <div class="d-flex justify-content-center align-items-center gap-2 mb-2">
        <img src="/assets/WEB/HOME/Phone big 2 Icon.svg" width="20" />
        <h3 class="mb-0">862-233-8330</h3>
      </div>
      <div class="d-flex justify-content-center align-items-center gap-2 mb-4">
        <img src="/assets/WEB/HOME/Location.svg" width="20" />
        <p class="mb-0">
          16 Chestnut Avenue Suite 2, Emerson, New Jersey 07630
        </p>
      </div>

      <div class="bg-black text-white py-4 mt-5">
        <img
          src="/assets/WEB/HOME/Logo Redeemed Blanco.png"
          height="40"
          class="mb-3"
        />
        <div class="mb-3 small">
          <a href="#" class="text-white mx-2 text-decoration-none">HOME</a>
          <a href="#" class="text-white mx-2 text-decoration-none">ABOUT US</a>
          <a href="#" class="text-white mx-2 text-decoration-none">SERVICES</a>
          <a href="#" class="text-white mx-2 text-decoration-none">DOWNLOAD</a>
          <a href="#" class="text-white mx-2 text-decoration-none"
            >CONTACT US</a
          >
          <a href="#" class="text-white mx-2 text-decoration-none">BLOG</a>
        </div>
        <div class="social-icons">
          <img
            src="/assets/WEB/HOME/Facebook Icon.svg"
            width="20"
            class="mx-2"
          />
          <img
            src="/assets/WEB/HOME/Twiiter icon.svg"
            width="20"
            class="mx-2"
          />
          <img
            src="/assets/WEB/HOME/Youtube icon.svg"
            width="20"
            class="mx-2"
          />
        </div>
      </div>
    </BContainer>
  </footer>
</template>
