<template>
  <div class="main-container">
    <div class="main-wrapper">
      <div class="left-wrapper">
        <img src="../assets/images/company-card.png" />
      </div>
      <div class="right-wrapper">
        <h1>Get in touch</h1>
        <div class="find-us">
          <h2>Find us</h2>
          <p>16 emenike Street, Mile 3 diobu, port Harcourt.</p>
          <a href="https://www.google.com/maps/place/Cobef+International+Limited/@4.860476,7.0854776,1125m/data=!3m2!1e3!4b1!4m6!3m5!1s0x1069d2ad21ae86bd:0x46fb3e4446572965!8m2!3d4.860476!4d7.0880525!16s%2Fg%2F11hzhc6m0m!5m1!1e1?entry=ttu&g_ep=EgoyMDI2MDkzMC4wIKXMDSoASAFQAw%3D%3D"
            target="_blank" class="button">
            View in Maps
          </a>
        </div>
        <div class="enquiry">
          <h2>Have an enquiry?</h2>
          <p>Whether you have a question about a future project, want to know more about how
            we work or are interested in a career with us, you can email us or give us a call by
            using the links below.
          </p>
        </div>
        <div class="links">
          <div class="telephone">
            <h2>Phone</h2>
            <i class="uil uil-phone" /><a href="tel:+2348124640233">+(234) 812-464-0233</a><br>
            <i class="uil uil-phone" /><a href="tel:+2348144425129">+(234) 814-442-5129</a><br>
          </div>
          <div class="email">
            <h2>Email</h2>
            <i class="uil uil-envelope" />
            <a href="mailto:diliforgeservicesltd@outlook.com">diliforgeservicesltd@outlook.com</a><br>
          </div>
          <div class="social">
            <h2>Socials</h2>
            <i class="uil uil-instagram"></i>
            <a href="https://instagram.com/diliforge" target="_blank">Diliforge</a><br>
            <i class="uil uil-twitter"></i>
            <a href="https://x.com/DILIFORGE_Ltd" target="_blank">DILIFORGE_Ltd
            </a><br>
            <i class="uil uil-music-note"></i>
            <a href="https://www.tiktok.com/@diliforge.service" target="_blank">diliforge.service</a>
          </div>
        </div>
      </div>
    </div>
    <div class="footer">
      <span>
        © Diliforge Services Limited. 2026
      </span>
    </div>
  </div>
</template>

<style scoped>
  .main-container {
    display: flex;
    flex-direction: column;
    padding: 20px 45px;
    background-color: var(--prybackground);
  }

  .main-wrapper {
    display: grid;
    grid-template-columns: minmax(0, 2fr) minmax(320px, 1fr);
    gap: 30px;
    align-items: start;
  }

  .left-wrapper {
    width: 100%;
    height: 100%;
  }

  .left-wrapper img {
    width: 100%;
    height: auto;
    display: block;
    object-fit: contain;
    border-radius: var(--border-radius);
  }

  .right-wrapper {
    width: 100%;
    min-width: 0;
  }

  .right-wrapper i {
    width: 23px;
    height: 23px;
    text-align: center;
    font-size: 14px;
    margin-bottom: .7em;
    color: var(--text);
  }

  .right-wrapper h1 {
    color: var(--prytext);
    font-size: clamp(2rem, 4vw, 4ch);
    margin-bottom: 4px;
    text-transform: capitalize;
    font-weight: 400;
  }

  .find-us,
  .links,
  .enquiry {
    margin-bottom: 1.4em;
    border-top: var(--border);
  }

  .find-us h2,
  .enquiry h2,
  .links h2 {
    font-weight: 400;
    font-size: 1.8ch;
    margin-bottom: 6px;
    margin-top: 10px;
    text-transform: capitalize;
    color: var(--prytext);
  }

  .find-us p,
  .enquiry p {
    font-size: .8em;
    margin-bottom: 20px;
    color: var(--sectext);
  }

  .find-us a {
    border: 1px solid #eeeeee5c;
    padding: 10px;
    margin: 0;
    color: var(--prytext);
    font-size: .8em;
    border-radius: var(--border-radius);
    letter-spacing: 1px;
    display: inline-block;
  }

  .find-us a:hover {
    background-color: var(--secbackground);
    color: var(--text);
  }

  .links a {
    font-weight: 300;
    color: var(--sectext);
    font-size: .8em;
    letter-spacing: 1px;
    margin-left: 7px;
    line-height: 2em;
    word-break: break-word;
  }

  .links a:hover {
    color: var(--text);
  }

  .links .telephone,
  .email {
    border-bottom: var(--border);
  }

  .social a {
    text-transform: lowercase;
  }

  .footer {
    width: 100%;
    font-size: 1.2ch;
    font-weight: bold;
    margin-top: 5px;
  }

  .footer span {
    color: #ffffff;
  }

  @media (max-width: 1024px) {
    .main-wrapper {
      grid-template-columns: 1.4fr 1fr;
      gap: 20px;
    }

    .links a {
      letter-spacing: .5px;
    }
  }

  @media (max-width: 768px) {
    .main-container {
      padding: 20px 45px;
    }

    .main-wrapper {
      grid-template-columns: 1fr;
      gap: 25px;
    }

    .left-wrapper {
      order: 1;
    }

    .right-wrapper {
      order: 2;
    }

    .right-wrapper h1 {
      font-size: 2rem;
    }

    .links a {
      font-size: .75em;
    }

    .footer span {
      font-size: 11px;
      text-align: center;
      display: block;
    }
  }

  @media (max-width: 480px) {
    .main-container {
      padding: 20px;
    }

    .right-wrapper h1 {
      font-size: 1.8rem;
    }

    .find-us a {
      width: 100%;
      text-align: center;
      box-sizing: border-box;
    }

    .links a {
      font-size: .7em;
      letter-spacing: 0;
    }
  }
</style>