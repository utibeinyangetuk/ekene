<template>
  <div class="main-wrapper">
    <div class="hero-wrapper">
      <div class="hero">
        <LandingPage />
      </div>
    </div>
    <ServicesPage />
    <FoundationPage />
    <ContactPage />
  </div>
</template>
<script setup>
  import ContactPage from './views/ContactPage.vue';
  import FoundationPage from './views/FoundationPage.vue';
  import LandingPage from './views/LandingPage.vue';
  import ServicesPage from './views/ServicesPage.vue';
</script>
<style>
  @import url("https://fonts.cdnfonts.com/css/poppins");

  :root {
    --prybackground: #350105;
    --secbackground: #cd8026;
    --text: #ffffff;
    --prytext: #cd8026;
    --sectext: #eae2e298;
    --border: 1px solid #eeeeee37;
    --border-radius: 5px;
    --padding: 50px;
  }

  #app {
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    overflow: auto;
    scroll-behavior: smooth;
    height: 95vh;
    border-radius: var(--border-radius);
  }

  body {
    padding: var(--padding);
  }

  * {
    font-family: 'poppins', sans-serif;
    margin: 0 auto;
    box-sizing: border-box;
    text-decoration: none;
    list-style: none;

    ::-webkit-scrollbar {
      width: 5px;
      display: none;
    }

    ::-webkit-scrollbar-track {
      background: var(--prybackground);
    }

    ::-webkit-scrollbar-thumb {
      background: var(--secbackground);
      border-radius: var(--border-radius);
    }
  }

  .hero-wrapper {
    padding: 50px;
    background: var(--prybackground);
  }

  .hero {
    position: relative;
  }

  @media only screen and (max-width: 768px) {
    .hero-wrapper {
      padding: 10px;
    }

    body {
      padding: 5px;
    }
  }

</style>