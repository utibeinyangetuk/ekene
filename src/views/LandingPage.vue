<script setup>
  import image1 from "../assets/images/image1.jpg";
  import image10 from "../assets/images/image10.jpg";
  import image11 from "../assets/images/image11.jpg";
  import image12 from "../assets/images/image12.jpg";
  import image2 from "../assets/images/image2.jpg";
  import image3 from "../assets/images/image3.jpg";
  import image4 from "../assets/images/image4.jpg";
  import image5 from "../assets/images/image5.jpg";
  import image6 from "../assets/images/image6.jpg";
  import image7 from "../assets/images/image7.jpg";
  import image8 from "../assets/images/image8.jpg";
  import image9 from "../assets/images/image9.jpg";
  // import logo from "../assets/images/logo.jpg";
  import Carousel from "../components/Carousel.vue";

  const slides = [
    image1,
    image2,
    image3,
    image4,
    image5,
    image6,
    image7,
    image8, image9, image10, image11, image12
  ];
</script>

<template>
  <header class="hero">
    <!-- <img :src="logo" class="site-logo" alt="Logo" /> -->
    <Carousel :images="slides" :interval="5000" :pagination="true" />
  </header>
  <div class="content">
    <h1>Integrated Solutions. Lasting Impacts.</h1>
    <p>
      <span style="color:var(--secbackground); font-weight: 800; letter-spacing: 1px;">Diliforge Services Limited</span>
      is a dynamic and diversified service company committed to delivering integrated
      solutions across multiple sectors. We provide professional services in drilling, manpower supply, procurement,
      logistics, construction support, branding, painting, HVAC, plumbing, importation,oil & gas support, and
      agricultural services.
      At Diliforge, we believe that successful projects are built on reliability, professionalism, quality, safety, and
      strong partnerships. Our approach combines practical expertise, responsive service delivery, and a clear
      understanding of our clients' needs to provide solutions that create measurable and lasting value.
      From technical and field services to procurement, logistics and project support, we are positioned to serve
      individuals, businesses, contractors, organizations, and communities with solutions tailored to their specific
      requirements.
      Our commitment is simple: deliver quality solutions, build lasting relationships, and create lasting impact.
    </p>
  </div>
</template>
<style scoped>
  .hero {
    position: relative;
  }

  /* .site-logo {
    position: absolute;
    top: 25px;
    left: 40px;
    width: 100px;
    z-index: 100;
    height: 100px;
  } */
  .content {
    display: grid;
    grid-template-columns: repeat(auto-fit,
        minmax(300px, 1fr));
    max-width: 1500px;
    margin: 0 auto;
    padding: 4rem 0rem;
    gap: 1rem;

  }

  .content h1 {
   font-size: 2rem;
    font-weight: 400;
    line-height: 1.2;
    margin-bottom: 1rem;
    color: var(--secbackground, #222);
    text-transform: uppercase;
    letter-spacing: 1px;
  }

  .content p {
   font-size: 1.3ch;
    line-height: 1.8;
    color: var(--text, #666);
    margin: 0;
    text-align: left;

  }

  @media (max-width: 768px) {
    .content {
      padding: 2rem 1rem;
    }

    .content h1 {
      font-size: 1.8rem;
      width: 100%;
    }

    .content p {
      font-size: 0.9rem;
    }
  }

  @media (max-width: 480px) {
    .content {
      padding: 1rem;
    }

    .content h1 {
      font-size: 1.5rem;
    }

    .content p {
      font-size: 0.8rem;
    }
  }
</style>