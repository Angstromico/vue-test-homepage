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
              <p class="text-muted small">USA 06/17/2021</p>
              <p>
                Lorem Ipsum Is Simply Dummy Text Of The Printing And Typesetting
                Industry. Lorem Ipsum Has Been The Industry's Standard Dummy
                Text Ever Since The 1500S,
              </p>
              <BButton variant="outline-primary" size="sm" class="rounded-pill"
                >View More</BButton
              >
            </BCardBody>
          </BCard>
        </BCol>
      </BRow>
    </BContainer>
  </section>
</template>
