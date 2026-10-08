# thepainthouse06
welcome to my github profile.
<br>
auther-bittu kumar
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>The Paint House | Professional Painting Services</title>

  <meta name="description"
        content="The Paint House provides professional interior, exterior and wall texture painting services.">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f8f9fa;
      color: #222;
      line-height: 1.6;
    }

    /* NAVBAR */
    header {
      background: #111;
      color: white;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 3px 15px rgba(0,0,0,0.2);
    }

    .navbar {
      max-width: 1200px;
      margin: auto;
      padding: 15px 25px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 27px;
      font-weight: bold;
    }

    .logo span {
      color: #ffb703;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 25px;
    }

    nav a {
      color: white;
      text-decoration: none;
      font-weight: 500;
      transition: 0.3s;
    }

    nav a:hover {
      color: #ffb703;
    }

    .menu-btn {
      display: none;
      font-size: 28px;
      cursor: pointer;
    }

    /* HERO */
    .hero {
      min-height: 90vh;
      display: flex;
      align-items: center;
      background:
        linear-gradient(rgba(0,0,0,.65), rgba(0,0,0,.65)),
        url("https://images.unsplash.com/photo-1562259949-e8e7689d7828?auto=format&fit=crop&w=1600&q=80")
        center/cover;
      color: white;
    }

    .hero-content {
      max-width: 1200px;
      width: 100%;
      margin: auto;
      padding: 40px 25px;
    }

    .hero h1 {
      font-size: clamp(42px, 7vw, 75px);
      line-height: 1.05;
      margin-bottom: 20px;
    }

    .hero h1 span {
      color: #ffb703;
    }

    .hero p {
      max-width: 650px;
      font-size: 20px;
      margin-bottom: 30px;
      color: #eee;
    }

    .btn {
      display: inline-block;
      background: #ffb703;
      color: #111;
      padding: 14px 28px;
      border-radius: 30px;
      text-decoration: none;
      font-weight: bold;
      margin-right: 10px;
      transition: .3s;
    }

    .btn:hover {
      transform: translateY(-3px);
      background: white;
    }

    .btn-outline {
      background: transparent;
      color: white;
      border: 2px solid white;
    }

    /* GENERAL */
    section {
      padding: 80px 25px;
    }

    .container {
      max-width: 1200px;
      margin: auto;
    }

    .section-title {
      text-align: center;
      margin-bottom: 50px;
    }

    .section-title h2 {
      font-size: 40px;
      margin-bottom: 10px;
    }

    .section-title span {
      color: #ff9800;
    }

    .section-title p {
      color: #666;
    }

    /* ABOUT */
    .about {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 50px;
      align-items: center;
    }

    .about img {
      width: 100%;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0,0,0,.15);
    }

    .about-text h2 {
      font-size: 40px;
      margin-bottom: 20px;
    }

    .about-text p {
      color: #555;
      margin-bottom: 20px;
    }

    .features {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 15px;
      margin-top: 25px;
    }

    .feature {
      padding: 15px;
      background: #fff;
      border-radius: 10px;
      box-shadow: 0 5px 20px rgba(0,0,0,.07);
    }

    .feature strong {
      color: #ff9800;
    }

    /* SERVICES */
    .services {
      background: #f1f3f5;
    }

    .service-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 25px;
    }

    .service-card {
      background: white;
      border-radius: 18px;
      overflow: hidden;
      box-shadow: 0 8px 25px rgba(0,0,0,.08);
      transition: .3s;
    }

    .service-card:hover {
      transform: translateY(-8px);
    }

    .service-card img {
      width: 100%;
      height: 220px;
      object-fit: cover;
    }

    .service-content {
      padding: 25px;
    }

    .service-content h3 {
      margin-bottom: 10px;
      font-size: 23px;
    }

    .service-content p {
      color: #666;
    }

    /* STATS */
    .stats {
      background: #111;
      color: white;
    }

    .stats-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
      text-align: center;
    }

    .stat h3 {
      font-size: 45px;
      color: #ffb703;
    }

    .stat p {
      color: #ddd;
    }

    /* GALLERY */
    .gallery-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 15px;
    }

    .gallery-grid img {
      width: 100%;
      height: 250px;
      object-fit: cover;
      border-radius: 12px;
      transition: .3s;
    }

    .gallery-grid img:hover {
      transform: scale(1.03);
    }

    /* WHY US */
    .why-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .why-card {
      text-align: center;
      padding: 30px 20px;
      background: white;
      border-radius: 15px;
      box-shadow: 0 5px 20px rgba(0,0,0,.08);
    }

    .why-icon {
      font-size: 45px;
      margin-bottom: 15px;
    }

    .why-card h3 {
      margin-bottom: 10px;
    }

    .why-card p {
      color: #666;
    }

    /* REVIEWS */
    .reviews {
      background: #f1f3f5;
    }

    .review-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 25px;
    }

    .review {
      background: white;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 5px 20px rgba(0,0,0,.07);
    }

    .stars {
      color: #ffb703;
      font-size: 20px;
      margin-bottom: 15px;
    }

    .review p {
      color: #555;
      margin-bottom: 15px;
    }

    .review h4 {
      color: #222;
    }

    /* CONTACT */
    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 50px;
    }

    .contact-info h2 {
      font-size: 40px;
      margin-bottom: 20px;
    }

    .contact-item {
      margin: 20px 0;
      font-size: 18px;
    }

    .contact-item strong {
      color: #ff9800;
    }

    form {
      background: #111;
      padding: 30px;
      border-radius: 18px;
    }

    form input,
    form textarea,
    form select {
      width: 100%;
      padding: 14px;
      margin-bottom: 15px;
      border: none;
      border-radius: 8px;
      outline: none;
    }

    form textarea {
      height: 130px;
      resize: vertical;
    }

    form button {
      border: none;
      cursor: pointer;
      width: 100%;
    }

    /* FOOTER */
    footer {
      background: #0a0a0a;
      color: white;
      padding: 40px 25px 20px;
    }

    .footer-grid {
      max-width: 1200px;
      margin: auto;
      display: grid;
      grid-template-columns: 2fr 1fr 1fr;
      gap: 40px;
    }

    footer h3 {
      margin-bottom: 15px;
      color: #ffb703;
    }

    footer p,
    footer a {
      color: #bbb;
      text-decoration: none;
    }

    footer a:hover {
      color: #ffb703;
    }

    .copyright {
      text-align: center;
      border-top: 1px solid #333;
      margin-top: 30px;
      padding-top: 20px;
      color: #888;
    }

    /* WHATSAPP */
    .whatsapp {
      position: fixed;
      right: 20px;
      bottom: 20px;
      width: 58px;
      height: 58px;
      border-radius: 50%;
      background: #25D366;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      text-decoration: none;
      font-size: 28px;
      box-shadow: 0 5px 20px rgba(0,0,0,.25);
      z-index: 999;
    }

    /* RESPONSIVE */
    @media (max-width: 900px) {

      .menu-btn {
        display: block;
      }

      nav ul {
        display: none;
        position: absolute;
        top: 68px;
        left: 0;
        width: 100%;
        background: #111;
        flex-direction: column;
        padding: 20px;
        text-align: center;
      }

      nav ul.active {
        display: flex;
      }

      .about,
      .contact-grid {
        grid-template-columns: 1fr;
      }

      .service-grid,
      .review-grid {
        grid-template-columns: 1fr 1fr;
      }

      .why-grid {
        grid-template-columns: 1fr 1fr;
      }

      .stats-grid {
        grid-template-columns: 1fr 1fr;
      }

      .gallery-grid {
        grid-template-columns: 1fr 1fr;
      }

      .footer-grid {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 600px) {

      section {
        padding: 60px 18px;
      }

      .hero {
        min-height: 80vh;
      }

      .hero p {
        font-size: 17px;
      }

      .btn {
        display: block;
        text-align: center;
        margin-bottom: 12px;
      }

      .service-grid,
      .review-grid,
      .why-grid,
      .gallery-grid,
      .stats-grid {
        grid-template-columns: 1fr;
      }

      .features {
        grid-template-columns: 1fr;
      }

      .section-title h2 {
        font-size: 32px;
      }
    }
  </style>
</head>

<body>

<!-- NAVBAR -->
<header>
  <div class="navbar">

    <div class="logo">
      The <span>Paint House</span>
    </div>

    <div class="menu-btn" onclick="toggleMenu()">☰</div>

    <nav>
      <ul id="navMenu">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#gallery">Gallery</a></li>
        <li><a href="#reviews">Reviews</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>

  </div>
</header>


<!-- HERO -->
<section class="hero" id="home">

  <div class="hero-content">

    <h1>
      Give Your Home<br>
      A <span>Beautiful Color</span>
    </h1>

    <p>
      Professional painting services for homes, offices and commercial
      spaces. Quality work, beautiful finishes and trusted service.
    </p>

    <a href="#contact" class="btn">Get Free Quote</a>
    <a href="#services" class="btn btn-outline">Our Services</a>

  </div>

</section>


<!-- ABOUT -->
<section id="about">

  <div class="container">

    <div class="about">

      <img
        src="https://images.unsplash.com/photo-1562259949-e8e7689d7828?auto=format&fit=crop&w=1000&q=80"
        alt="Professional painting">

      <div class="about-text">

        <h2>About <span>The Paint House</span></h2>

        <p>
          The Paint House is a professional painting service dedicated
          to transforming homes and commercial spaces with beautiful,
          long-lasting finishes.
        </p>

        <p>
          Our team focuses on quality preparation, clean workmanship,
          reliable service and customer satisfaction.
        </p>

        <div class="features">

          <div class="feature">
            ✓ <strong>Professional Team</strong>
          </div>

          <div class="feature">
            ✓ <strong>Quality Materials</strong>
          </div>

          <div class="feature">
            ✓ <strong>Clean Work</strong>
          </div>

          <div class="feature">
            ✓ <strong>On-Time Service</strong>
          </div>

        </div>

      </div>

    </div>

  </div>

</section>


<!-- SERVICES -->
<section class="services" id="services">

  <div class="container">

    <div class="section-title">
      <h2>Our <span>Painting Services</span></h2>
      <p>Professional solutions for every space.</p>
    </div>

    <div class="service-grid">

      <div class="service-card">

        <img
          src="https://images.unsplash.com/photo-1562259949-e8e7689d7828?auto=format&fit=crop&w=800&q=80"
          alt="Interior painting">

        <div class="service-content">
          <h3>Interior Painting</h3>
          <p>
            Give your rooms a fresh and beautiful look with
            professional interior wall painting.
          </p>
        </div>

      </div>


      <div class="service-card">

        <img
          src="https://images.unsplash.com/photo-1600566753086-00f18fb6b3ea?auto=format&fit=crop&w=800&q=80"
          alt="Exterior painting">

        <div class="service-content">
          <h3>Exterior Painting</h3>
          <p>
            Durable exterior painting designed to improve
            the appearance of your property.
          </p>
        </div>

      </div>


      <div class="service-card">

        <img
          src="https://images.unsplash.com/photo-1618220179428-22790b461013?auto=format&fit=crop&w=800&q=80"
          alt="Wall texture">

        <div class="service-content">
          <h3>Wall Texture Design</h3>
          <p>
            Modern and attractive wall textures for stylish
            interiors and feature walls.
          </p>
        </div>

      </div>


      <div class="service-card">

        <img
          src="https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?auto=format&fit=crop&w=800&q=80"
          alt="Home painting">

        <div class="service-content">
          <h3>Home Painting</h3>
          <p>
            Complete painting solutions for apartments,
            houses and villas.
          </p>
        </div>

      </div>


      <div class="service-card">

        <img
          src="https://images.unsplash.com/photo-1497366754035-f200968a6e72?auto=format&fit=crop&w=800&q=80"
          alt="Office painting">

        <div class="service-content">
          <h3>Office Painting</h3>
          <p>
            Professional office painting to create a fresh
            and welcoming workspace.
          </p>
        </div>

      </div>


      <div class="service-card">

        <img
          src="https://images.unsplash.com/photo-1600210492486-724fe5c67fb0?auto=format&fit=crop&w=800&q=80"
          alt="Decorative painting">

        <div class="service-content">
          <h3>Decorative Painting</h3>
          <p>
            Creative decorative finishes that add character
            and style to your space.
          </p>
        </div>

      </div>

    </div>

  </div>

</section>


<!-- STATS -->
<section class="stats">

  <div class="container">

    <div class="stats-grid">

      <div class="stat">
        <h3>500+</h3>
        <p>Projects Completed</p>
      </div>

      <div class="stat">
        <h3>10+</h3>
        <p>Years Experience</p>
      </div>

      <div class="stat">
        <h3>450+</h3>
        <p>Happy Customers</p>
      </div>

      <div class="stat">
        <h3>100%</h3>
        <p>Quality Focus</p>
      </div>

    </div>

  </div>

</section>


<!-- GALLERY -->
<section id="gallery">

  <div class="container">

    <div class="section-title">
      <h2>Our <span>Work Gallery</span></h2>
      <p>Some examples of painting and interior work.</p>
    </div>

    <div class="gallery-grid">

      <img src="https://images.unsplash.com/photo-1600210492486-724fe5c67fb0?auto=format&fit=crop&w=800&q=80" alt="Painting work">

      <img src="https://images.unsplash.com/photo-1600566753086-00f18fb6b3ea?auto=format&fit=crop&w=800&q=80" alt="Home interior">

      <img src="https://images.unsplash.com/photo-1618220179428-22790b461013?auto=format&fit=crop&w=800&q=80" alt="Wall design">

      <img src="https://images.unsplash.com/photo-1600607687920-4e2a09cf159d?auto=format&fit=crop&w=800&q=80" alt="Interior design">

      <img src="https://images.unsplash.com/photo-1600607688969-a5bfcd646154?auto=format&fit=crop&w=800&q=80" alt="Room painting">

      <img src="https://images.unsplash.com/photo-1600607687920-4e2a09cf159d?auto=format&fit=crop&w=800&q=80" alt="House painting">

    </div>

  </div>

</section>


<!-- WHY CHOOSE US -->
<section>

  <div class="container">

    <div class="section-title">
      <h2>Why <span>Choose Us?</span></h2>
      <p>We focus on quality, service and customer satisfaction.</p>
    </div>

    <div class="why-grid">

      <div class="why-card">
        <div class="why-icon">🎨</div>
        <h3>Expert Painters</h3>
        <p>Skilled professionals for quality finishing.</p>
      </div>

      <div class="why-card">
        <div class="why-icon">⭐</div>
        <h3>Quality Work</h3>
        <p>Attention to detail on every project.</p>
      </div>

      <div class="why-card">
        <div class="why-icon">⏱️</div>
        <h3>On-Time</h3>
        <p>We respect your time and project schedule.</p>
      </div>

      <div class="why-card">
        <div class="why-icon">💰</div>
        <h3>Fair Pricing</h3>
        <p>Transparent pricing for your painting needs.</p>
      </div>

    </div>

  </div>

</section>


<!-- REVIEWS -->
<section class="reviews" id="reviews">

  <div class="container">

    <div class="section-title">
      <h2>Customer <span>Reviews</span></h2>
      <p>What our customers say.</p>
    </div>

    <div class="review-grid">

      <div class="review">
        <div class="stars">★★★★★</div>
        <p>
          "Very professional work. The finishing was clean
          and our home looks completely different."
        </p>
        <h4>— Customer 1</h4>
      </div>

      <div class="review">
        <div class="stars">★★★★★</div>
        <p>
          "Good service and excellent communication.
          The team completed the work on time."
        </p>
        <h4>— Customer 2</h4>
      </div>

      <div class="review">
        <div class="stars">★★★★★</div>
        <p>
          "The wall texture design came out beautifully.
          Very happy with the final result."
        </p>
        <h4>— Customer 3</h4>
      </div>

    </div>

  </div>

</section>


<!-- CONTACT -->
<section id="contact">

  <div class="container">

    <div class="contact-grid">

      <div class="contact-info">

        <h2>Let's <span style="color:#ff9800;">Paint Your Space</span></h2>

        <p>
          Have a painting project? Contact us for a free
          consultation and quotation.
        </p>

        <div class="contact-item">
          📞 <strong>Phone:</strong> +91 9798376390
        </div>

        <div class="contact-item">
          📧 <strong>Email:</strong> rkraj4102@gmail.com
        </div>

        <div class="contact-item">
          📍 <strong>Location:</strong> Chewara,Sheikhpura (Bihar) 811304
        </div>

      </div>


      <form onsubmit="sendMessage(event)">

        <input type="text" id="name"
               placeholder="Your Name" required>

        <input type="tel" id="phone"
               placeholder="Phone Number" required>

        <select id="service" required>

          <option value="">Select Service</option>
          <option>Interior Painting</option>
          <option>Exterior Painting</option>
          <option>Wall Texture</option>
          <option>Home Painting</option>
          <option>Office Painting</option>
          <option>Decorative Painting</option>

        </select>

        <textarea id="message"
                  placeholder="Tell us about your project..."
                  required></textarea>

        <button class="btn" type="submit">
          Send Enquiry
        </button>

      </form>

    </div>

  </div>

</section>


<!-- FOOTER -->
<footer>

  <div class="footer-grid">

    <div>
      <h3>The Paint House</h3>
      <p>
        Professional painting services for homes,
        offices and commercial spaces.
      </p>
    </div>

    <div>
      <h3>Quick Links</h3>
      <p><a href="#home">Home</a></p>
      <p><a href="#about">About</a></p>
      <p><a href="#services">Services</a></p>
      <p><a href="#contact">Contact</a></p>
    </div>

    <div>
      <h3>Services</h3>
      <p>Interior Painting</p>
      <p>Exterior Painting</p>
      <p>Wall Texture</p>
      <p>Home Painting</p>
    </div>

  </div>

  <div class="copyright">
    © 2026 The Paint House. All Rights Reserved.
  </div>

</footer>


<!-- WHATSAPP BUTTON -->
<a
  class="whatsapp"
  href="https://wa.me/919798376390"
  target="_blank"
  aria-label="Chat on WhatsApp">
  ☎
</a>


<script>

  /* MOBILE MENU */
  function toggleMenu() {

    const menu = document.getElementById("navMenu");

    menu.classList.toggle("active");

  }


  /* CONTACT FORM */
  function sendMessage(event) {

    event.preventDefault();

    const name =
      document.getElementById("name").value;

    const phone =
      document.getElementById("phone").value;

    const service =
      document.getElementById("service").value;

    const message =
      document.getElementById("message").value;


    /*
      IMPORTANT:
      Replace 919798376390 with
      your actual WhatsApp number.
    */

    const whatsappNumber = "919798376390";

    const text =
      `Hello The Paint House,%0A%0A` +
      `Name: ${name}%0A` +
      `Phone: ${phone}%0A` +
      `Service: ${service}%0A` +
      `Message: ${message}`;


    window.open(
      `https://wa.me/${whatsappNumber}?text=${text}`,
      "_blank"
    );

  }

</script>

</body>
</html>
```

