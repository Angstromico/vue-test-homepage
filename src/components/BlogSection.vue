<script setup lang="ts">
import {
  BContainer,
  BRow,
  BCol,
  BCard,
  BCardBody,
  BButton,
} from 'bootstrap-vue-next'
</script>

<template>
  <section class="blog-section py-5 bg-light">
    <BContainer>
      <h2 class="text-center mb-5">BLOG</h2>
      <BRow>
        <BCol md="4" class="mb-4" v-for="i in 3" :key="i">
          <BCard no-body class="h-100 border-0 shadow-sm">
            <img
              src="/assets/WEB/HOME/Picture Blog Home.png"
              class="card-img-top"
            />
            <BCardBody class="text-center">
              <h5>Lorem Ipsum</h5>
              <p class="text-muted small">July 2024</p>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
              <BButton variant="outline-primary" size="sm" class="rounded-pill"
                >Read More</BButton
              >
            </BCardBody>
          </BCard>
        </BCol>
      </BRow>
    </BContainer>
  </section>
</template>
