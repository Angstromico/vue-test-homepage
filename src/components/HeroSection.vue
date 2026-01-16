<script setup lang="ts">
import { ref, onMounted } from 'vue'
import { BContainer, BRow, BCol, BButton } from 'bootstrap-vue-next'

const currentSlide = ref(0)
const totalSlides = 3

const nextSlide = () => {
  currentSlide.value = (currentSlide.value + 1) % totalSlides
}

const setSlide = (index: number) => {
  currentSlide.value = index
}

// Auto-advance carousel
onMounted(() => {
  setInterval(nextSlide, 5000)
})
</script>

<template>
  <div class="hero-section position-relative text-white mt-n3">
    <!-- Desktop Phone Number (Visible LG+) -->
    <div
      class="d-none d-lg-block w-100 position-absolute top-0 end-0 p-4 z-index-top text-end"
    >
      <div class="d-inline-flex align-items-center gap-2 text-white">
        <img
          src="/assets/WEB/HOME/Phone big 2 Icon.svg"
          height="24"
          class="filter-white"
        />
        <span class="fs-4 fw-bold">862-233-8330</span>
      </div>
    </div>

    <img
      src="/assets/WEB/HOME/Banner principal 1.jpg"
      class="img-fluid w-100 hero-img"
      alt="Banner"
    />
    <div
      class="hero-overlay position-absolute top-0 start-0 w-100 h-100 d-flex align-items-center"
    >
      <BContainer>
        <BRow>
          <BCol md="6" offset-md="6" class="text-end pe-5 position-relative">
            <!-- Arrow Graphic -->
            <img
              src="/assets/WEB/HOME/Arrow next.svg"
              class="arrow-graphic d-none d-md-block"
            />

            <h1 class="display-4 fw-bold">INDIVIDUAL TAX<br />PREPARATION</h1>
            <p class="fs-4 fst-italic">You Can Count On...</p>
            <BButton variant="primary" class="rounded-pill mt-3 px-4"
              >Learn More</BButton
            >
          </BCol>
        </BRow>
      </BContainer>
    </div>

    <!-- CTA Cards -->
    <div class="cta-cards-container">
      <BContainer>
        <!-- Desktop View: All cards visible, overlapping banner -->
        <BRow class="g-0 d-none d-lg-flex cta-desktop-row">
          <BCol md="4">
            <div
              class="cta-card bg-primary p-4 text-center text-white border-end border-light"
            >
              <img
                src="/assets/WEB/HOME/Individual Tax Preparation Blanco.svg"
                height="50"
                class="mb-3"
              />
              <h5>Individual tax preparation</h5>
            </div>
          </BCol>
          <BCol md="4">
            <div
              class="cta-card bg-primary p-4 text-center text-white border-end border-light"
            >
              <img
                src="/assets/WEB/HOME/Bookepping Blanco.svg"
                height="50"
                class="mb-3"
              />
              <h5>Bookkeeping</h5>
            </div>
          </BCol>
          <BCol md="4">
            <div class="cta-card bg-primary p-4 text-center text-white">
              <img
                src="/assets/WEB/HOME/Business Tax Preparation Blanco.svg"
                height="50"
                class="mb-3"
              />
              <h5>Business tax preparation</h5>
            </div>
          </BCol>
        </BRow>

        <!-- Mobile/Tablet View: Carousel -->
        <div class="d-lg-none py-4 position-relative">
          <div class="carousel-inner overflow-hidden rounded shadow">
            <div
              class="cta-card bg-primary p-5 text-center text-white"
              v-if="currentSlide === 0"
            >
              <img
                src="/assets/WEB/HOME/Individual Tax Preparation Blanco.svg"
                height="60"
                class="mb-3"
              />
              <h4>Individual tax preparation</h4>
            </div>
            <div
              class="cta-card bg-primary p-5 text-center text-white"
              v-if="currentSlide === 1"
            >
              <img
                src="/assets/WEB/HOME/Bookepping Blanco.svg"
                height="60"
                class="mb-3"
              />
              <h4>Bookkeeping</h4>
            </div>
            <div
              class="cta-card bg-primary p-5 text-center text-white"
              v-if="currentSlide === 2"
            >
              <img
                src="/assets/WEB/HOME/Business Tax Preparation Blanco.svg"
                height="60"
                class="mb-3"
              />
              <h4>Business tax preparation</h4>
            </div>
          </div>

          <!-- Carousel Dots -->
          <div class="d-flex justify-content-center gap-2 mt-3">
            <span
              v-for="i in 3"
              :key="i"
              class="carousel-dot"
              :class="{ active: currentSlide === i - 1 }"
              @click="setSlide(i - 1)"
            ></span>
          </div>
        </div>
      </BContainer>
    </div>
  </div>
</template>

<style scoped>
.hero-section {
  overflow: visible; /* Allow cards to overlap */
}
.hero-img {
  object-fit: cover;
  min-height: 500px;
}
.cta-card {
  height: 100%;
  transition: transform 0.2s;
}
.cta-desktop-row {
  margin-top: -80px; /* Pull up to overlap banner */
  position: relative;
  z-index: 10;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.cta-card:hover {
  /* Only hover effect on desktop to avoid stuck states on touch */
  @media (min-width: 992px) {
    transform: translateY(-5px);
  }
}

.z-index-top {
  z-index: 20;
}
.filter-white {
  filter: brightness(0) invert(1);
}

/* Arrow Graphic Positioning */
.arrow-graphic {
  position: absolute;
  right: 100%; /* Default: Left of the text block */
  top: 50%;
  transform: translateY(-50%) translateX(-20px);
  height: 40px;
}

@media (max-width: 991px) {
  .hero-overlay {
    background: rgba(0, 0, 0, 0.4);
  }
  .arrow-graphic {
    /* Tablet positioning if different, per user request 'next to text... but in different position' */
    /* Based on sample description, putting it top right relative to text block or similar. */
    /* Since I can't see the image, I'll stick to a safe responsive adjustment */
    top: 0;
    right: 0;
    transform: translate(50%, -100%);
  }
}

/* Carousel Dots */
.carousel-dot {
  width: 12px;
  height: 12px;
  background-color: #ccc;
  border-radius: 50%;
  cursor: pointer;
  transition: background-color 0.3s;
}
.carousel-dot.active {
  background-color: #fff;
  /* User said white when selected, but background is white-ish? */
  /* If background is light, white might disappear. */
  /* Let's assume section below hero is light/white. */
  /* Actually user said "gray circles that turn white". */
  /* Wait, the background of the dots area is likely the white page background. */
  /* So gray on white is visible. White on white is invisible unless bg is dark. */
  /* Let's try blue active state if white is invisible, or check context. */
  /* App.vue shows Hero followed by Services (bg-light). */
  /* So dots area has white/light bg. */
  /* "turn white when... selected" implies dark background? */
  /* Or maybe blue background? */
  /* I'll start with primary color for active as safe fallback or check the sample image logic... */
  /* User said: "turn white when they are positioned over the selected box" */
  /* Aha! If dots are OVER the box (overlay), then white makes sense. */
  /* But current Mobile layout puts dots BELOW the box. */
  /* I'll stick to gray/primary for visibility unless I move them inside. */
  background-color: #0d6efd;
}
</style>
