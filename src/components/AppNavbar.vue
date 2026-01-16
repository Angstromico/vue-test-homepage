<script setup lang="ts">
import {
  BNavbar,
  BContainer,
  BNavbarBrand,
  BNavbarToggle,
  BCollapse,
  BNavbarNav,
  BNavItem,
  BButton,
} from 'bootstrap-vue-next'
</script>

<template>
  <BNavbar
    toggleable="lg"
    class="py-3 custom-navbar border-bottom border-white"
    fixed="top"
  >
    <BContainer>
      <!-- Phone Number for Mobile/Tablet (Hidden on Large screens) -->
      <div
        class="d-lg-none w-100 text-center mb-3 text-white d-flex justify-content-center align-items-center gap-2"
      >
        <img
          src="/assets/WEB/HOME/Phone big 2 Icon.svg"
          height="20"
          class="filter-white"
        />
        <span class="fs-5 fw-bold">862-233-8330</span>
      </div>

      <BNavbarBrand href="#">
        <img
          src="/assets/WEB/HOME/Logo Redeemed Header.png"
          alt="Logo"
          height="70"
        />
      </BNavbarBrand>

      <BNavbarToggle target="nav-collapse" class="border-white" />

      <BCollapse id="nav-collapse" is-nav>
        <BNavbarNav class="ms-auto align-items-center gap-3">
          <BNavItem href="#" class="nav-link-custom">HOME</BNavItem>
          <BNavItem href="#" class="nav-link-custom">ABOUT US</BNavItem>
          <BNavItem href="#" class="nav-link-custom">SERVICES</BNavItem>
          <BNavItem href="#" class="nav-link-custom">DOWNLOAD</BNavItem>
          <BNavItem href="#" class="nav-link-custom">BLOG</BNavItem>

          <!-- Contact Us Button -->
          <BNavItem>
            <BButton
              variant="info"
              class="contact-btn rounded-pill px-4 text-white fw-bold"
              >Contact Us</BButton
            >
          </BNavItem>

          <!-- Register Button -->
          <BNavItem>
            <BButton variant="dark" class="rounded px-4 text-white fw-bold"
              >REGISTER</BButton
            >
          </BNavItem>

          <!-- Login Image -->
          <BNavItem href="#">
            <img
              src="/assets/WEB/HOME/LOGIN ICON.svg"
              height="40"
              alt="Login"
            />
          </BNavItem>

          <!-- Flags (Stacked) -->
          <BNavItem>
            <div class="d-flex flex-column align-items-center gap-1">
              <img
                src="/assets/WEB/HOME/united-states-of-america.svg"
                height="20"
                alt="English"
              />
              <img src="/assets/WEB/HOME/spain.svg" height="20" alt="Spanish" />
            </div>
          </BNavItem>
        </BNavbarNav>
      </BCollapse>
    </BContainer>
  </BNavbar>
</template>

<style scoped>
/* Navbar Transparency and Text */
.custom-navbar {
  background-color: transparent !important;
  transition: background-color 0.3s;
}

/* Ensure text is white */
:deep(.nav-link),
:deep(.navbar-toggler-icon) {
  color: white !important;
  font-weight: 500;
}
:deep(.navbar-toggler) {
  filter: invert(1);
  border-color: white !important;
}

.nav-link-custom {
  font-size: 0.9rem;
  letter-spacing: 0.5px;
}

.contact-btn {
  background-color: #0dcaf0; /* Light blue */
  border: none;
  text-transform: none; /* Mixed case */
}

/* Force white icons on mobile if needed */
.filter-white {
  filter: brightness(0) invert(1);
}

@media (max-width: 991px) {
  /* Add background on mobile so menu is readable */
  .custom-navbar {
    background-color: rgba(0, 0, 0, 0.9) !important;
  }
}
</style>
