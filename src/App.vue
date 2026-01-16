<script setup lang="ts">
import AppNavbar from './components/AppNavbar.vue'
import HeroSection from './components/HeroSection.vue'
import ServicesSection from './components/ServicesSection.vue'
import InfoSection from './components/InfoSection.vue'
import TestimonialsSection from './components/TestimonialsSection.vue'
import ContactBar from './components/ContactBar.vue'
import BlogSection from './components/BlogSection.vue'
import AppFooter from './components/AppFooter.vue'
</script>

<template>
  <main style="width: 100vw">
    <AppNavbar />
    <HeroSection />
    <ServicesSection />
    <InfoSection />
    <TestimonialsSection />
    <ContactBar />
    <BlogSection />
    <AppFooter />
  </main>
</template>
