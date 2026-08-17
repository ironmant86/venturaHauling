<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Ventura – Hauling & Junk Removal</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content="Ventura – fast, reliable hauling and junk removal services in Ventura County." />
  <style>
    :root {
      --primary: #1f6feb;
      --accent: #f4b41a;
      --dark: #1b1b1f;
      --light: #f7f7f9;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: var(--light);
      color: var(--dark);
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    header {
      background: var(--dark);
      color: #fff;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .nav {
      max-width: 1100px;
      margin: 0 auto;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0.75rem 1rem;
    }

    .logo {
      font-weight: 700;
      letter-spacing: 0.08em;
      text-transform: uppercase;
    }

    .logo span {
      color: var(--accent);
    }

    .nav-links {
      display: flex;
      gap: 1rem;
      font-size: 0.95rem;
    }

    .nav-links a {
      padding: 0.25rem 0.5rem;
      border-radius: 4px;
    }

    .nav-links a:hover {
      background: rgba(255, 255, 255, 0.1);
    }

    .btn-primary {
      background: var(--primary);
      color: #fff;
      border-radius: 4px;
      padding: 0.6rem 1.1rem;
      border: none;
      cursor: pointer;
      font-weight: 600;
      font-size: 0.95rem;
    }

    .btn-primary:hover {
      background: #1551b3;
    }

    .hero {
      background: linear-gradient(135deg, #1f6feb, #163b73);
      color: #fff;
      padding: 3.5rem 1rem;
    }

    .hero-inner {
      max-width: 1100px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: minmax(0, 2fr) minmax(0, 1.5fr);
      gap: 2rem;
      align-items: center;
    }

    .hero h1 {
      font-size: 2.4rem;
      margin-bottom: 0.75rem;
    }

    .hero h2 {
      font-size: 1.2rem;
      font-weight: 500;
      margin-bottom: 1rem;
    }

    .hero p {
      margin-bottom: 1.25rem;
    }

    .hero-list {
      list-style: none;
      margin-bottom: 1.5rem;
    }

    .hero-list li::before {
      content: "✔";
      color: var(--accent);
      margin-right: 0.4rem;
      font-weight: 700;
    }

    .hero-contact {
      font-size: 0.95rem;
      margin-top: 0.75rem;
    }

    .hero-card {
      background: rgba(255, 255, 255, 0.08);
      border-radius: 10px;
      padding: 1.5rem;
      border: 1px solid rgba(255, 255, 255, 0.2);
    }

    .hero-card h3 {
      margin-bottom: 0.75rem;
      font-size: 1.1rem;
    }

    .hero-card p {
      font-size: 0.9rem;
      margin-bottom: 0.5rem;
    }

    main {
      max-width: 1100px;
      margin: 0 auto;
      padding: 2.5rem 1rem 3rem;
    }

    section {
      margin-bottom: 3rem;
    }

    section h2 {
      font-size: 1.8rem;
      margin-bottom: 0.75rem;
    }

    section p.section-intro {
      margin-bottom: 1.5rem;
      color: #555;
      font-size: 0.98rem;
    }

    .grid-2 {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 1.5rem;
    }

    .card {
      background: #fff;
      border-radius: 8px;
      padding: 1.25rem;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.04);
      border: 1px solid #e3e3ea;
    }

    .card h3 {
      font-size: 1.1rem;
      margin-bottom: 0.5rem;
    }

    .card ul {
      list-style: none;
      font-size: 0.95rem;
    }

    .card ul li {
      margin-bottom: 0.35rem;
    }

    .card ul li::before {
      content: "•";
      color: var(--primary);
      margin-right: 0.4rem;
    }

    .pricing-table {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 1.5rem;
    }

    .price-card {
      background: #fff;
      border-radius: 8px;
      padding: 1.25rem;
      border: 1px solid #e3e3ea;
      text-align: center;
    }

    .price-card h3 {
      margin-bottom: 0.5rem;
    }

    .price-range {
      font-size: 1.1rem;
      font-weight: 600;
      color: var(--primary);
      margin-bottom: 0.5rem;
    }

    .price-note {
      font-size: 0.9rem;
      color: #666;
    }

    .about-layout {
      display: grid;
      grid-template-columns: minmax(0, 2fr) minmax(0, 1.5fr);
      gap: 1.5rem;
    }

    .pill-list {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      margin-top: 0.75rem;
    }

    .pill-list li {
      background: #fff;
      border-radius: 999px;
      padding: 0.35rem 0.75rem;
      border: 1px solid #e3e3ea;
      font-size: 0.85rem;
    }

    .contact-layout {
      display: grid;
      grid-template-columns: minmax(0, 1.5fr) minmax(0, 2fr);
      gap: 1.5rem;
    }

    .contact-info p {
      font-size: 0.95rem;
      margin-bottom: 0.4rem;
    }

    .service-area {
      font-size: 0.9rem;
      color: #555;
      margin-top: 0.5rem;
    }

    form {
      background: #fff;
      border-radius: 8px;
      padding: 1.5rem;
      border: 1px solid #e3e3ea;
    }

    .form-row {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 1rem;
      margin-bottom: 1rem;
    }

    label {
      display: block;
      font-size: 0.85rem;
      margin-bottom: 0.25rem;
      color: #444;
    }

    input,
    textarea {
      width: 100%;
      padding: 0.5rem 0.6rem;
      border-radius: 4px;
      border: 1px solid #cfd2e3;
      font-size: 0.9rem;
      font-family: inherit;
    }

    textarea {
      min-height: 100px;
      resize: vertical;
    }

    footer {
      background: var(--dark);
      color: #aaa;
      font-size: 0.85rem;
      padding: 1.25rem 1rem;
      margin-top: 1rem;
    }

    .footer-inner {
      max-width: 1100px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 0.75rem;
    }

    .footer-inner a {
      color: #ddd;
      font-size: 0.85rem;
    }

    @media (max-width: 768px) {
      .hero-inner,
      .about-layout,
      .contact-layout {
        grid-template-columns: 1fr;
      }

      .nav {
        flex-wrap: wrap;
        gap: 0.75rem;
      }

      .nav-links {
        flex-wrap: wrap;
        justify-content: flex-end;
      }

      .hero {
        padding: 2.5rem 1rem;
      }

      .hero h1 {
        font-size: 2rem;
      }
    }
  </style>
</head>
<body>
  <!-- Header / Navigation -->
  <header>
    <div class="nav">
      <div class="logo">
        Ventura <span>Hauling and Junk Removal</span>
      </div>
      <nav class="nav-links">
        <a href="#home">Home</a>
        <a href="#services">Services</a>
        <a href="#pricing">Pricing</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <!-- Hero / Home -->
  <section id="home" class="hero">
    <div class="hero-inner">
      <div>
        <h1>Ventura Hauling & Junk Removal</h1>
        <h2>Fast • Reliable • Local</h2>
        <p>
          Your trusted hauling and junk‑removal team serving Ventura County and surrounding areas.
          From single‑item pickups to full property cleanouts, Ventura delivers fast, affordable,
          and dependable service every time.
        </p>
        <ul class="hero-list">
          <li>Same‑day & next‑day service</li>
          <li>Residential & commercial hauling</li>
          <li>Fully insured</li>
          <li>Free estimates</li>
        </ul>
        <button class="btn-primary" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">
          Get a Free Estimate
        </button>
        <div class="hero-contact">
          <p><strong>Call:</strong> (805) 732‑4739</p>
          <p><strong>Email:</strong> venturahauling8@gmail.com</p>
          <p><strong>Hours:</strong> 7 AM – 7 PM, 7 days a week</p>
        </div>
      </div>
      <div class="hero-card">
        <h3>Why Choose Ventura Hauling and Junk Removal?</h3>
        <p>• Friendly local crew that treats your property with respect.</p>
        <p>• Transparent pricing with no hidden fees.</p>
        <p>• Eco‑friendly disposal whenever possible.</p>
        <p>• Serving Ventura, Oxnard, Camarillo, Port Hueneme, Santa Paula, Ojai, and nearby cities.</p>
      </div>
    </div>
  </section>

  <main>
    <!-- Services -->
    <section id="services">
      <h2>Services</h2>
      <p class="section-intro">
        No job is too big or too small—Ventura handles it all. We offer full‑service hauling and junk removal
        for homes, businesses, and construction sites.
      </p>
      <div class="grid-2">
        <div class="card">
          <h3>Junk Removal</h3>
          <ul>
            <li>Household clutter</li>
            <li>Furniture & appliances</li>
            <li>Mattresses</li>
            <li>Yard waste</li>
            <li>Garage cleanouts</li>
          </ul>
        </div>
        <div class="card">
          <h3>Hauling Services</h3>
          <ul>
            <li>Construction debris</li>
            <li>Dirt, rock, and green waste</li>
            <li>Scrap metal</li>
            <li>Bulk item transport</li>
          </ul>
        </div>
        <div class="card">
          <h3>Property Cleanouts</h3>
          <ul>
            <li>Rental units</li>
            <li>Storage units</li>
            <li>Foreclosures</li>
            <li>Estate cleanouts</li>
          </ul>
        </div>
        <div class="card">
          <h3>Commercial Services</h3>
          <ul>
            <li>Office cleanouts</li>
            <li>Retail waste removal</li>
            <li>Warehouse debris hauling</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- Pricing -->
    <section id="pricing">
      <h2>Pricing</h2>
      <p class="section-intro">
        We use simple, volume‑based pricing so you always know what to expect. Final quotes depend on load size,
        material type, and access.
      </p>
      <div class="pricing-table">
        <div class="price-card">
          <h3>Small Load</h3>
          <div class="price-range">$99 – $150</div>
          <p class="price-note">Perfect for single items or small piles.</p>
        </div>
        <div class="price-card">
          <h3>Medium Load</h3>
          <div class="price-range">$150 – $300</div>
          <p class="price-note">Ideal for room cleanouts or mixed junk.</p>
        </div>
        <div class="price-card">
          <h3>Large Load</h3>
          <div class="price-range">$300 – $600</div>
          <p class="price-note">Great for garage, yard, or multi‑room cleanouts.</p>
        </div>
        <div class="price-card">
          <h3>Full Trailer</h3>
          <div class="price-range">Custom Quote</div>
          <p class="price-note">For major projects and construction debris.</p>
        </div>
      </div>
      <p class="section-intro">
        Heavy materials (dirt, concrete, tile) may include a surcharge. After‑hours pickups are available upon request.
        Send us photos or schedule an on‑site visit for a free estimate.
      </p>
    </section>



    <!-- About -->
    <section id="about">
      <h2>About Ventura</h2>
      <div class="about-layout">
        <div>
          <p class="section-intro">
            Ventura Hauling Services was built on a simple idea: provide honest, hardworking hauling services
            that treat every customer like a neighbor. We’re a local team committed to keeping our community clean,
            organized, and stress‑free.
          </p>
          <p>
            From the first phone call to the final sweep‑up, we focus on clear communication, fair pricing,
            and respect for your time and property. We show up when we say we will, work efficiently,
            and leave your space looking better than we found it.
          </p>
        </div>
        <div>
          <h3>Our Values</h3>
          <ul class="pill-list">
            <li>Reliability</li>
            <li>Fair Pricing</li>
            <li>Respect for Your Property</li>
            <li>Eco‑Friendly Disposal</li>
            <li>Local Community Focus</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact">
      <h2>Contact</h2>
      <div class="contact-layout">
        <div class="contact-info">
          <p><strong>Phone:</strong> (805) 732‑4739</p>
          <p><strong>Email:</strong> venturahauling8@gmail.com</p>
          <p><strong>Service Area:</strong> Ventura County, Oxnard, Camarillo, Port Hueneme, Santa Paula, Ojai, and nearby cities.</p>
          <p class="service-area">
            Send us a message with a brief description of what you need hauled, and we’ll get back to you with
            a free estimate—often the same day.
          </p>
        </div>
        <form>
          <div class="form-row">
            <div>
              <label for="name">Name</label>
              <input id="name" name="name" type="text" placeholder="Your name" />
            </div>
            <div>
              <label for="phone">Phone</label>
              <input id="phone" name="phone" type="tel" placeholder="(805) 732‑4739" />
            </div>
          </div>
          <div class="form-row">
            <div>
              <label for="email">Email</label>
              <input id="email" name="email" type="email" placeholder="you@example.com" />
            </div>
            <div>
              <label for="address">Address / City</label>
              <input id="address" name="address" type="text" placeholder="City or full address" />
            </div>
          </div>
          <div class="form-row">
            <div style="grid-column: 1 / -1;">
              <label for="description">Description of Items</label>
              <textarea id="description" name="description" placeholder="Tell us what needs to be hauled, approximate volume, and any access details."></textarea>
            </div>
          </div>
          <div class="form-row">
            <div>
              <label for="date">Preferred Date</label>
              <input id="date" name="date" type="date" />
            </div>
            <div>
              <label for="time">Preferred Time</label>
              <input id="time" name="time" type="time" />
            </div>
          </div>
          <button type="submit" class="btn-primary">Submit Request</button>
        </form>
      </div>
    </section>
  </main>

  <!-- Footer -->
  <footer>
    <div class="footer-inner">
      <div>© <span id="year"></span> Ventura Hauling & Junk Removal. All rights reserved.</div>
      <div>
        <a href="#home">Back to top</a>
      </div>
    </div>
  </footer>

  <script>
    // Set current year in footer
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
