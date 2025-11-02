# filamatrix-website
3D printer filament
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Filamatrix | Premium 3D Printer Filaments</title>

  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');
    * {
      margin: 0; padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }
    body {
      font-family: 'Poppins', sans-serif;
      background-color: #f9fbff;
      color: #222;
      line-height: 1.6;
    }

    header {
      background: linear-gradient(135deg, #0077b6, #00b4d8);
      color: white;
      padding: 1.5rem 5%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0; z-index: 10;
    }

    header h1 {
      font-size: 1.8rem;
      font-weight: 700;
    }

    nav a {
      color: white;
      margin: 0 12px;
      text-decoration: none;
      font-weight: 500;
      transition: 0.3s;
    }

    nav a:hover { color: #ffdd57; }

    /* Hero Section */
    .hero {
      background: url('https://images.unsplash.com/photo-1616628188500-5b4c85f2d9a7?auto=format&fit=crop&w=1600&q=80') center/cover no-repeat;
      color: white;
      text-align: center;
      padding: 8rem 2rem;
      position: relative;
    }
    .hero::after {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0; bottom: 0;
  background: url('https://th.bing.com/th/id/OIP.ZIinrF0FUrsV6en-zxC6aQHaE8?w=308&h=180&c=7&r=0&o=7&dpr=1.3&pid=1.7&rm=3')
              center/cover no-repeat;
  opacity: 0.6; /* optional: makes it partially visible for blending */
  }

    .hero-content {
      position: relative; z-index: 2;
    }
    .hero h2 { font-size: 3rem; margin-bottom: 1rem; }
    .hero p { font-size: 1.2rem; margin-bottom: 2rem; }
    .hero a {
      background: #ffdd57; color: #000;
      padding: 0.8rem 1.5rem; border-radius: 30px;
      font-weight: 600; text-decoration: none;
      transition: 0.3s;
    }
    .hero a:hover { background: #fff; }

    section {
      padding: 5rem 10%;
    }

    h2.section-title {
      text-align: center;
      font-size: 2rem;
      color: #0077b6;
      margin-bottom: 2rem;
    }

    /* About */
    .about p {
      font-size: 1.1rem;
      margin-bottom: 1.5rem;
      text-align: justify;
      color: #444;
    }

    .vision {
      background: #e3f7ff;
      padding: 3rem;
      border-radius: 10px;
      margin-bottom: 3rem;
    }
    .vision h3 {
      color: #0077b6;
      margin-bottom: 1rem;
    }

    /* Materials */
    .materials ul {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      list-style: none;
      gap: 2rem;
    }
    .materials li {
      background: #fff;
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0,0,0,0.05);
      width: 250px;
      text-align: center;
      padding: 1.5rem;
      transition: 0.3s;
    }
    .materials li:hover { transform: translateY(-5px); }
    .materials li h4 { color: #0077b6; margin-bottom: 0.5rem; }

    /* Products */
    .products {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 2rem;
    }
    .product {
      background: #fff;
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0,0,0,0.1);
      width: 300px;
      text-align: center;
      overflow: hidden;
      transition: 0.3s;
    }
    .product:hover { transform: translateY(-5px); }
    .product img {
      width: 100%; height: 200px;
      object-fit: cover;
    }
    .product h4 { color: #0077b6; padding: 1rem 0; }

    /* Why & Support */
    .why, .support {
      background: #eaf7ff;
      padding: 3rem;
      border-radius: 10px;
      margin-top: 3rem;
    }
    .why ul, .support ul {
      list-style: disc;
      margin-left: 2rem;
      color: #444;
      line-height: 1.8;
    }

    /* Contact */
    .contact-info {
      text-align: center;
      margin-bottom: 2rem;
      font-size: 1.1rem;
      color: #333;
    }

    form {
      max-width: 500px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }
    input, textarea {
      padding: 0.8rem;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-family: inherit;
      font-size: 1rem;
    }
    button {
      background: #0077b6;
      color: white;
      padding: 0.8rem;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: 0.3s;
    }
    button:hover { background: #00b4d8; }

    footer {
      background: #222;
      color: white;
      text-align: center;
      padding: 1.5rem;
      margin-top: 3rem;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .materials ul, .products {
        flex-direction: column;
        align-items: center;
      }
      .hero h2 { font-size: 2rem; }
    }
  </style>
</head>
<body>

  <header>
    <h1>Filamatrix</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#vision">Vision</a>
      <a href="#materials">Materials</a>
      <a href="#products">Products</a>
      <a href="#support">Support</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-content">
      <h2>Print the Future with Filamatrix</h2>
      <p>Premium, high-performance 3D printing filaments engineered for makers, creators, and professionals.</p>
      <a href="#products">Explore Our Range</a>
    </div>
  </section>

  <section id="about" class="about">
    <h2 class="section-title">About Us</h2>
    <p>At <strong>Filamatrix</strong>, we believe in empowering creativity through precision and quality. We are a next-generation manufacturer of 3D printer filaments that combine cutting-edge technology with eco-friendly materials. Our research team continuously improves formulations to ensure consistency, reliability, and superior color performance.</p>
    <p>We serve industries from prototyping to manufacturing, ensuring every print meets the highest standards. Our focus on sustainable materials and innovation helps drive the next wave of 3D printing excellence.</p>
  </section>

  <section id="vision" class="vision">
    <h2 class="section-title">Our Vision & Mission</h2>
    <h3>Vision:</h3>
    <p>To redefine 3D printing materials through sustainable, high-performance filaments that bring digital creations to life.</p>
    <h3>Mission:</h3>
    <p>To deliver precision-engineered filaments with unparalleled quality, making 3D printing more accessible and eco-conscious for everyone.</p>
  </section>

  <section id="materials" class="materials">
    <h2 class="section-title">Materials We Use</h2>
    <ul>
      <li><h4>PLA</h4><p>Eco-friendly, biodegradable, easy to print — perfect for beginners and artistic models.</p></li>
      <li><h4>PETG</h4><p>Combines strength and flexibility — ideal for mechanical and functional parts.</p></li>
      <li><h4>ABS</h4><p>Durable and heat-resistant — great for industrial-grade projects.</p></li>
      <li><h4>TPU</h4><p>Flexible and strong — ideal for wearable or shock-absorbing components.</p></li>
      <li><h4>Carbon Fiber</h4><p>Ultra-rigid, lightweight material designed for aerospace and automotive applications.</p></li>
    </ul>
  </section>

  <section id="products">
    <h2 class="section-title">Our Product Range</h2>
    <div class="products">
      <div class="product">
        <img src="https://th.bing.com/th/id/OIP.aoU19W5SRAOyCR-9cYojawHaHa?w=165&h=180&c=7&r=0&o=7&dpr=1.3&pid=1.7&rm=3">
        <h4>PLA Filament</h4>
        <p>Available in 20+ colors with glossy finish and smooth extrusion.</p>
      </div>
      <div class="product">
        <img src="https://th.bing.com/th/id/OIP.eut85dZ0EMrHwruBOMlM_gHaHa?w=187&h=187&c=7&r=0&o=7&dpr=1.3&pid=1.7&rm=3">
        <h4>PETG Filament</h4>
        <p>Strong, reliable, and moisture-resistant filament for durable parts.</p>
      </div>
      <div class="product">
        <img src="https://th.bing.com/th/id/OIP.w7TCo7tnREb9s-_lYZ7l7AHaHa?w=187&h=187&c=7&r=0&o=7&dpr=1.3&pid=1.7&rm=3">
        <h4>Carbon Fiber Reinforced</h4>
        <p>Lightweight, high-strength material perfect for engineering use.</p>
      </div>
    </div>
  </section>

  <section class="why">
    <h2 class="section-title">Why Choose Filamatrix?</h2>
    <ul>
      <li>Consistent filament diameter for precision prints</li>
      <li>Environmentally conscious and recyclable spools</li>
      <li>Compatible with most 3D printers</li>
      <li>Fast global shipping and support</li>
      <li>Vibrant color palette and specialty materials</li>
    </ul>
  </section>

  <section id="support" class="support">
    <h2 class="section-title">Customer Support</h2>
    <ul>
      <li>24/7 chat and email support</li>
      <li>Guides for printer calibration and optimal settings</li>
      <li>Replacement warranty for manufacturing defects</li>
    </ul>
  </section>

  <section id="contact">
    <h2 class="section-title">Contact Us</h2>
    <div class="contact-info">
      <p><strong>📧 Email:</strong> filamatrix@gmail.com</p>
      <p><strong>📱 Phone:</strong> +91 9878675676</p>
    </div>
    <form>
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Filamatrix — Precision in Every Layer | Contact: filamatrix@gmail.com | +91 9878675676</p>
  </footer>

</body>
</html>
