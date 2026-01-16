<script setup lang="ts">
import { BContainer, BRow, BCol } from 'bootstrap-vue-next'
</script>

<template>
  <section class="contact-bar py-4 bg-dark text-white">
    <BContainer>
      <BRow class="align-items-center">
        <BCol md="4">
          <h4 class="mb-0">Contact Us!</h4>
          <small
            >There are many variations of passages of Lorem Ipsum but the
            majority have suffered alteration.</small
          >
        </BCol>
        <BCol md="8">
          <div class="input-group">
            <input
              type="email"
              class="form-control rounded-pill"
              placeholder="Email here"
            />
            <button class="btn btn-primary rounded-pill ms-2" type="button">
              Send
            </button>
          </div>
        </BCol>
      </BRow>
    </BContainer>
  </section>
</template>
