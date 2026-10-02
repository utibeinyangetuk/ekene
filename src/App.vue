<template>
  <div class="main-wrapper">
    <div class="hero-wrapper">
      <div class="hero">
        <LandingPage />
      </div>
    </div>
  </div>

</template>
<script setup>
  import LandingPage from './views/LandingPage.vue';
</script>
<style>
  @import url("https://fonts.cdnfonts.com/css/poppins");

  :root {
    --prybackground: #7B1E3C;
    --secbackground: #C5A253;
    --text: #EDEEE7;
    /*
    --background4: #F2EBDB;
    --background5: #ADB3C2; */
    --prytext: #231F20;
    --sectext: #FDF5E5;
    --border: 1px solid #000000;
    --box-shadow: -4px 8px 0 0 var(--secbackground);
    --border-radius: 8px;
    --padding: 15px;
  }

  #app {
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    overflow: auto;
    scroll-behavior: smooth;
    height: 98vh;
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
  }

</style>