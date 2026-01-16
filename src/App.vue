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
  BRow,
  BCol,
  BCard,
  BCardBody,
} from 'bootstrap-vue-next'
</script>

<template>
  <div>
    <!-- Navbar -->
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

    <!-- Hero Section -->
    <div class="hero-section position-relative text-white mt-5 pt-4">
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
            <BCol md="6" offset-md="6" class="text-end pe-5">
              <h1 class="display-4 fw-bold">INDIVIDUAL TAX<br />PREPARATION</h1>
              <p class="fs-4 fst-italic">You Can Count On...</p>
              <BButton variant="primary" class="rounded-pill mt-3 px-4"
                >Learn More</BButton
              >
            </BCol>
          </BRow>
        </BContainer>
      </div>

      <!-- CTA Cards (overlapping hero slightly) -->
      <div class="cta-cards-container">
        <BContainer>
          <BRow class="g-0">
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
        </BContainer>
      </div>
    </div>

    <!-- Services Section -->
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
          <div
            class="service-item position-absolute"
            style="top: 10%; left: 20%"
          >
            <img src="/assets/WEB/HOME/Personal Budgeting.png" width="100" />
            <p class="mt-2 fw-bold">Personal<br />Bookkeeping</p>
          </div>
          <!-- Middle Left -->
          <div
            class="service-item position-absolute"
            style="top: 40%; left: 15%"
          >
            <img src="/assets/WEB/HOME/Notary Services.png" width="100" />
            <p class="mt-2 fw-bold">Notary<br />Services</p>
          </div>
          <!-- Bottom Left -->
          <div
            class="service-item position-absolute"
            style="top: 70%; left: 20%"
          >
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

    <!-- Info Section -->
    <section class="info-section">
      <img
        src="/assets/WEB/HOME/Banner inferior Individual Business.jpg"
        class="w-100 img-fluid"
      />
    </section>

    <!-- Testimonials -->
    <section class="testimonials-section py-5 bg-primary text-white">
      <BContainer>
        <h2 class="text-center mb-5">TESTIMONIALS</h2>
        <BRow>
          <BCol md="4" class="mb-4" v-for="i in 3" :key="i">
            <BCard class="text-center h-100 text-dark">
              <img
                src="/assets/WEB/HOME/Testimonials Picture.png"
                class="rounded-circle mb-3"
                width="80"
              />
              <h5 class="fw-bold">Clara Smith</h5>
              <p class="text-muted small">CEO - Any Company</p>
              <hr />
              <p class="card-text">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </p>
              <BButton variant="primary" size="sm" class="rounded-pill mt-3"
                >Read More</BButton
              >
            </BCard>
          </BCol>
        </BRow>
      </BContainer>
    </section>

    <!-- Contact & Search -->
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

    <!-- Blog -->
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
                <BButton
                  variant="outline-primary"
                  size="sm"
                  class="rounded-pill"
                  >Read More</BButton
                >
              </BCardBody>
            </BCard>
          </BCol>
        </BRow>
      </BContainer>
    </section>

    <!-- Footer -->
    <footer class="footer py-5 text-center">
      <BContainer>
        <BButton variant="primary" size="lg" class="rounded-pill mb-4 px-5"
          >BOOK TODAY</BButton
        >
        <div
          class="d-flex justify-content-center align-items-center gap-2 mb-2"
        >
          <img src="/assets/WEB/HOME/Phone big 2 Icon.svg" width="20" />
          <h3 class="mb-0">862-233-8330</h3>
        </div>
        <div
          class="d-flex justify-content-center align-items-center gap-2 mb-4"
        >
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
            <a href="#" class="text-white mx-2 text-decoration-none"
              >ABOUT US</a
            >
            <a href="#" class="text-white mx-2 text-decoration-none"
              >SERVICES</a
            >
            <a href="#" class="text-white mx-2 text-decoration-none"
              >DOWNLOAD</a
            >
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
  </div>
</template>

<style scoped>
.hero-section {
  overflow: hidden;
}
.hero-img {
  object-fit: cover;
  min-height: 500px; /* Ensure height on mobile */
}

/* Custom Overrides for Primary Color if needed */
.bg-primary {
  background-color: #0d6efd !important; /* Adjust to match image blue */
}
.cta-card {
  height: 100%;
  transition: transform 0.2s;
}
.cta-card:hover {
  transform: translateY(-5px);
}

.service-item {
  width: 150px;
  text-align: center;
}

@media (max-width: 991px) {
  .hero-overlay {
    background: rgba(
      0,
      0,
      0,
      0.4
    ); /* Darken overly on mobile for readability */
  }
}
</style>
