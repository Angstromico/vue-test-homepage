<script setup lang="ts">
import { BContainer, BRow, BCol } from 'bootstrap-vue-next'
</script>

<template>
  <section class="contact-bar py-4 bg-dark text-white">
    <BContainer>
      <BRow class="align-items-center">
        <BCol md="4">
          <h4 class="mb-0">Contact Us!</h4>
          <small>Find out more about our services.</small>
        </BCol>
        <BCol md="8">
          <div class="input-group">
            <input
              type="text"
              class="form-control rounded-pill"
              placeholder="Search..."
            />
            <button class="btn btn-primary rounded-pill ms-2" type="button">
              Search
            </button>
          </div>
        </BCol>
      </BRow>
    </BContainer>
  </section>
</template>
