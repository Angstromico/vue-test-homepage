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
    type="light"
    variant="light"
    class="py-3 shadow-sm bg-white"
    fixed="top"
  >
    <BContainer>
      <BNavbarBrand href="#">
        <img
          src="/assets/WEB/HOME/Logo Redeemed Header.png"
          alt="Logo"
          height="50"
        />
      </BNavbarBrand>

      <BNavbarToggle target="nav-collapse" />

      <BCollapse id="nav-collapse" is-nav>
        <BNavbarNav class="ms-auto align-items-center">
          <BNavItem href="#">HOME</BNavItem>
          <BNavItem href="#">ABOUT US</BNavItem>
          <BNavItem href="#">SERVICES</BNavItem>
          <BNavItem href="#">RESOURCES</BNavItem>
          <BNavItem href="#">BLOG</BNavItem>
          <BNavItem>
            <BButton variant="primary" class="rounded-pill px-4 text-white"
              >BOOK TODAY</BButton
            >
          </BNavItem>
          <BNavItem href="#">Portal Login</BNavItem>
          <BNavItem>
            <div class="d-flex align-items-center gap-2">
              <img
                src="/assets/WEB/HOME/united-states-of-america.svg"
                height="20"
                alt="English"
              />
              <span>English</span>
            </div>
          </BNavItem>
        </BNavbarNav>
      </BCollapse>
    </BContainer>
  </BNavbar>
</template>
