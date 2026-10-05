<script setup>
  import image1 from "../assets/images/image1.jpg";
  import image10 from "../assets/images/image10.jpg";
  import image11 from "../assets/images/image11.jpg";
  import image12 from "../assets/images/image12.jpg";
  import image13 from "../assets/images/image13.jpg";
  import image14 from "../assets/images/image14.jpg";
  import image15 from "../assets/images/image15.jpg";
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
    image8, image9, image10, image11, image12, image13, image14, image15
  ];
</script>

<template>
 <header class="hero">
    <Carousel :images="slides" :interval="5000" :pagination="true" />
  </header>
 <div class="content">
   <div class="content-label">
      About Diliforge
    </div>

    <div class="content-text">
      <p>
       <span>
          Diliforge Services Limited
        </span>
        is a dynamic and diversified service company committed to delivering
        integrated solutions across multiple sectors. We provide professional
        services in drilling, manpower supply, procurement, logistics,
        construction support, branding, painting, HVAC, plumbing, importation,
        oil & gas support, and agricultural services.
      </p>
     <p>
        At Diliforge, we believe that successful projects are built on
        reliability, professionalism, quality, safety, and strong partnerships.
        Our approach combines practical expertise, responsive service delivery,
        and a deep understanding of our clients' needs to provide solutions that
        create measurable and lasting value.
      </p>

      <p>
        From technical and field services to procurement, logistics, and project
        support, we are positioned to serve individuals, businesses,
        contractors, organizations, and communities with solutions tailored to
        their specific requirements.
      </p>

      <p>
        Our commitment is simple: deliver quality solutions, build lasting
        relationships, and create lasting impact.
      </p>
    </div>
  </div>
</template>
<style scoped>
 .hero {
    position: relative;
   width: 100%;
  }

.content {
   margin: 0 auto;
    padding: 90px 45px;
    display: grid;
   grid-template-columns: 280px 1fr;
    gap: 60px;
  }

  .content-label {
    color: #b8860b;
    text-transform: uppercase;
    letter-spacing: 3px;
    font-size: .9rem;
    font-weight: 700;
    position: sticky;
    top: 100px;
    height: fit-content;
  }

  .content-text {
    border-left: 1px solid #ececec;
    padding-left: 40px;
  }

  .content-text p {
    color: #555;
    line-height: 2;
    font-size: 1rem;
    margin-bottom: 22px;
  }

.content-text p:last-child {
    margin-bottom: 0;
  }

.content-text span {
    color: var(--prytext);
    font-weight: 700;
    letter-spacing: .5px;
  }

@media (max-width: 1024px) {
    .content {
      grid-template-columns: 200px 1fr;
      gap: 40px;
    }

  .content-text {
      padding-left: 30px;
    }
  }

@media (max-width: 768px) {
    .content {
     grid-template-columns: 1fr;
      gap: 20px;
      padding: 60px 25px;
    }

  .content-label {
      position: static;
      margin-bottom: 10px;
    }

  .content-text {
      border-left: none;
      border-top: 2px solid #ececec;
      padding-left: 0;
      padding-top: 25px;
    }

    .content-text p {
      font-size: .95rem;
      line-height: 1.9;
    }
  }

@media (max-width: 480px) {
    .content {
     padding: 50px 20px;
      gap: 15px;
    }

  .content-label {
      font-size: .8rem;
      letter-spacing: 2px;
    }

  .content-text {
      padding-top: 20px;
    }

    .content-text p {
      font-size: .9rem;
      line-height: 1.8;
      margin-bottom: 18px;
    }
  }

</style>