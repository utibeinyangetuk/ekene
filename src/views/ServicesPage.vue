<template>
  <div class="container">
    <section class="services">
      <div class="services-header">
        <span>Our Services</span>
        <h1>Integrated Solutions. Lasting Impacts.</h1>
        <p>
          Diliforge Services Limited provides integrated solutions across
          procurement, logistics, technical support, construction, facility
          maintenance, manpower supply, and industrial services. We deliver
          reliable, efficient, and value-driven solutions tailored to the unique
          needs of our clients.
        </p>
      </div>

      <div class="services-grid">

        <div class="service-card">
          <div class="service-icon">
            <i class="uil uil-import"></i>
          </div>
          <h2>Importation & Procurement</h2>
          <p>
            Strategic sourcing, importation, procurement support, supplier
            engagement, and delivery of quality products for projects and
            operations.
          </p>
        </div>

        <div class="service-card">
          <div class="service-icon">
            <i class="uil uil-truck"></i>
          </div>
          <h2>Logistics, Haulage & Distribution</h2>
          <p>
            Efficient transportation, cargo movement, distribution planning,
            warehousing support, and end-to-end logistics coordination.
          </p>
        </div>

        <div class="service-card">
          <div class="service-icon">
            <i class="uil uil-users-alt"></i>
          </div>
          <h2>Manpower Supply</h2>
          <p>
            Provision of skilled, semi-skilled, and support personnel to meet
            operational, technical, and project workforce requirements.
          </p>
        </div>

        <div class="service-card">
          <div class="service-icon">
            <i class="uil uil-oil-rig"></i>
          </div>
          <h2>Drilling Services</h2>
          <p>
            Supporting drilling and industrial operations with dependable
            technical personnel, equipment coordination, and operational support.
          </p>
        </div>

        <div class="service-card">
          <div class="service-icon">
            <i class="uil uil-constructor"></i>
          </div>
          <h2>Construction Support</h2>
          <p>
            Construction assistance, project support, site coordination,
            materials management, and workforce deployment.
          </p>
        </div>

        <div class="service-card">
          <div class="service-icon">
            <i class="uil uil-wind"></i>
          </div>
          <h2>HVAC Services</h2>
          <p>
            Installation, servicing, maintenance, troubleshooting, and support
            for heating, ventilation, and air-conditioning systems.
          </p>
        </div>

        <div class="service-card">
          <div class="service-icon">
            <i class="uil uil-water"></i>
          </div>
          <h2>Plumbing Services</h2>
          <p>
            Professional plumbing installations, repairs, maintenance, and
            infrastructure support for residential and commercial facilities.
          </p>
        </div>

        <div class="service-card">
          <div class="service-icon">
            <i class="uil uil-paint-tool"></i>
          </div>
          <h2>Painting & Branding</h2>
          <p>
            Interior and exterior painting, facility beautification, branding,
            signage installation, and visual enhancement solutions.
          </p>
        </div>

        <div class="service-card">
          <div class="service-icon">
            <i class="uil uil-box"></i>
          </div>
          <h2>Supply Chain & Warehousing</h2>
          <p>
            Inventory support, storage solutions, supply chain coordination,
            material handling, and warehouse management services.
          </p>
        </div>

      </div>
    </section>
  </div>
</template>

<style scoped>
  .services {
    padding: 80px 45px;
    background: #ffffff;
  }

  .services-header {
    margin-bottom: 60px;
  }

  .services-header span {
    color: #b8860b;
    text-transform: uppercase;
    letter-spacing: 3px;
    font-size: .85rem;
    font-weight: 700;
  }

  .services-header h1 {
    color: #7a0116;
    font-size: clamp(2.5rem, 6vw, 4.5rem);
    line-height: 1.1;
    margin: 8px 0 20px;
    font-weight: 300;
  }

  .services-header p {
    color: #555;
    line-height: 1.9;
  }

  .services-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 30px;
  }

  .service-card {
    position: relative;
    background: #fff;
    padding: 40px;
    min-height: 200px;
    border-radius: var(--border-radius);
    overflow: hidden;
    transition: all .3s ease;
    border: 1px solid #dad8d8;
  }

  .service-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 25px 60px rgba(0, 0, 0, .08);
  }

  .service-card:hover::before {
    width: 12px;
    transition: .3s ease;
  }

  .service-card:hover .service-icon i {
    color: rgba(122, 1, 22, .15);
  }

  .service-icon {
    position: absolute;
    right: -3px;
    top: 5px;
    pointer-events: none;
  }

  .service-icon i {
    font-size: 7rem;
    color: rgba(122, 1, 22, .08);
  }

  `` .service-card h2 {
    position: relative;
    z-index: 2;
    color: #222;
    font-size: 1.45rem;
    line-height: 1.3;
    margin-bottom: 18px;
    font-weight: 500;
    max-width: 80%;
  }

  .service-card p {
    position: relative;
    z-index: 2;
    color: #666;
    line-height: 1.8;
    font-size: .92rem;
  }

  /* Tablet */
  @media (max-width: 1024px) {
    .services-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  /* Mobile */
  @media (max-width: 768px) {
    .services {
      padding: 60px 25px;
    }

    .services-grid {
      grid-template-columns: 1fr;
    }

    .service-card {
      padding: 25px;
    }

    .services-header h1 {
      font-size: 2.2rem;
    }
  }

  /* Small Phones */
  @media (max-width: 480px) {
    .services {
      padding: 50px 20px;
    }

    .services-header h1 {
      font-size: 2rem;
    }

    .service-card {
      padding: 20px;
    }

    .service-icon {
      width: 55px;
      height: 55px;
    }

    .service-icon i {
      font-size: 24px;
    }
  }
</style>