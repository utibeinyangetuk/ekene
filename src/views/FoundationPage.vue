<template>
  <div class="container">
    <section class="foundation">
      <div class="foundation-header">
        <span>Our Foundation</span>
        <h1>Built on Purpose, Driven by Excellence.</h1>
        <p>
          At Diliforge Services Limited, our foundation is shaped by a commitment
          to integrity, professionalism, innovation, and long-term value creation.
          These principles guide every decision we make, every project we undertake,
          and every relationship we build.
        </p>
      </div>

      <div class="foundation-grid">

        <div class="foundation-card">
          <span class="label">Our Mission</span>
          <h2>Delivering Solutions That Create Lasting Value</h2>
          <p>
            To deliver reliable, innovative, and cost-effective integrated
            solutions across diverse sectors by combining professional expertise,
            quality service, safety, and strategic partnerships to create lasting
            value for our clients and communities.
          </p>
        </div>

        <div class="foundation-card">
          <span class="label">Our Vision</span>
          <h2>Shaping a Trusted Future</h2>
          <p>
            To become a trusted and respected multi-sector service company
            recognized for excellence, integrity, innovation, and sustainable
            impact across Nigeria and beyond.
          </p>
        </div>

      </div>

      <div class="values-section">
        <div class="values-header">
          <span>Core Values</span>
          <h2>The Principles That Define Us</h2>
        </div>

        <div class="values-grid">

          <div class="value-card">
            <h3>Integrity</h3>
            <p>
              We conduct our business with honesty, transparency, and
              accountability in every engagement.
            </p>
          </div>

          <div class="value-card">
            <h3>Professionalism</h3>
            <p>
              We maintain high standards in how we work, communicate,
              and deliver value to our stakeholders.
            </p>
          </div>

          <div class="value-card">
            <h3>Safety</h3>
            <p>
              We prioritize the safety of our people, clients, assets,
              and the environment at all times.
            </p>
          </div>

          <div class="value-card">
            <h3>Quality</h3>
            <p>
              We are committed to delivering services that meet
              the highest standards and exceed expectations.
            </p>
          </div>

          <div class="value-card">
            <h3>Reliability</h3>
            <p>
              We strive to be a dependable partner from initial engagement
              through successful project completion.
            </p>
          </div>

          <div class="value-card">
            <h3>Innovation</h3>
            <p>
              We embrace practical ideas, modern approaches, and
              continuous improvement in solving challenges.
            </p>
          </div>

          <div class="value-card">
            <h3>Partnership</h3>
            <p>
              We build relationships based on trust, collaboration,
              mutual respect, and shared value creation.
            </p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
  .foundation {
    width: 100%;
    padding: 80px 45px;
    background: var(--prybackground);
  }

  .foundation-header {
    margin-bottom: 60px;
  }

  .foundation-header span,
  .values-header span {
    color: var(--accent, #d4af37);
    font-size: 0.85rem;
    letter-spacing: 2px;
    text-transform: uppercase;
    font-weight: 600;
  }

  .foundation-header h1 {
    color: var(--prytext);
    font-size: clamp(2.5rem, 6vw, 4.5rem);
    font-weight: 300;
    line-height: 1.1;
    margin: 12px 0 20px;
  }

  .foundation-header p {
    color: var(--sectext);
    line-height: 1.8;
    font-size: 1rem;
  }

  .foundation-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 30px;
    margin-bottom: 80px;
  }

  .foundation-card {
    border: var(--border);
    border-radius: var(--border-radius);
    padding: 35px;
    transition: 0.3s ease;
  }

  .foundation-card:hover {
    transform: translateY(-6px);
  }

  .foundation-card .label {
    display: inline-block;
    margin-bottom: 15px;
    color: var(--accent, #d4af37);
    text-transform: uppercase;
    letter-spacing: 2px;
    font-size: 0.8rem;
  }

  .foundation-card h2 {
    color: var(--prytext);
    font-size: 1.8rem;
    font-weight: 400;
    margin-bottom: 20px;
    line-height: 1.3;
  }

  .foundation-card p {
    color: var(--sectext);
    line-height: 1.8;
    font-size: 0.95rem;
  }

  .values-section {
    margin-top: 40px;
  }

  .values-header {
    margin-bottom: 40px;
  }

  .values-header h2 {
    color: var(--prytext);
    font-size: clamp(2rem, 4vw, 3rem);
    font-weight: 300;
    margin-top: 12px;
  }

  .values-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 25px;
  }

  .value-card {
    border: var(--border);
    border-radius: var(--border-radius);
    padding: 30px;
    transition: 0.3s ease;
  }

  .value-card:hover {
    background: rgba(255, 255, 255, 0.03);
    transform: translateY(-5px);
  }

  .value-card h3 {
    color: var(--prytext);
    font-size: 1.2rem;
    font-weight: 500;
    margin-bottom: 15px;
  }

  .value-card p {
    color: var(--sectext);
    line-height: 1.7;
    font-size: 0.92rem;
  }

  /* Tablet */
  @media (max-width: 1024px) {
    .foundation {
      padding: 60px 45px;
    }

    .foundation-grid {
      grid-template-columns: 1fr;
    }

    .values-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  /* Mobile */
  @media (max-width: 768px) {
    .foundation {
      padding: 50px 25px;
    }

    .foundation-header {
      margin-bottom: 40px;
    }

    .foundation-card {
      padding: 25px;
    }

    .values-grid {
      grid-template-columns: 1fr;
    }

    .value-card {
      padding: 25px;
    }

    .foundation-card h2 {
      font-size: 1.4rem;
    }

    .values-header h2 {
      font-size: 2rem;
    }
  }

  /* Small phones */
  @media (max-width: 480px) {
    .foundation {
      padding: 40px 20px;
    }

    .foundation-header h1 {
      font-size: 2rem;
    }

    .foundation-header p,
    .foundation-card p,
    .value-card p {
      font-size: 0.9rem;
    }

    .foundation-card,
    .value-card {
      padding: 20px;
    }
  }
</style>