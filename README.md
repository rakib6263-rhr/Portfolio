<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Rihan's Portfolio</title>

  <!-- Font Awesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" />

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      background: #f8f9fa;
      padding-top: 70px; /* Prevent navbar overlap */
    }

    /* Navbar */
    .navbar {
      background-color: #4a90e2;
      color: white;
      padding: 15px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 1000;
    }

    .navbar h2 {
      font-size: 22px;
    }

    .menu-icon {
      width: 30px;
      cursor: pointer;
    }

    .menu-icon div {
      background: white;
      height: 4px;
      margin: 5px 0;
      border-radius: 2px;
    }

    .nav-links {
      display: none;
      flex-direction: column;
      background: #357ABD;
      position: absolute;
      top: 60px;
      left: 0;
      width: 100%;
    }

    .nav-links a {
      color: white;
      text-decoration: none;
      padding: 15px 20px;
      border-top: 1px solid #4a90e2;
    }

    .nav-links a:hover {
      background: #28527a;
    }

    .nav-active {
      display: flex;
    }

    /* Sections */
    .section {
      padding: 100px 20px 60px;
      text-align: center;
    }

    .section h1, .section h2 {
      margin-bottom: 10px;
    }

    .section p {
      color: #555;
      font-size: 16px;
      max-width: 700px;
      margin: 0 auto;
    }

    /* Home Section */
    .home h1 {
      font-size: 32px;
      color: #333;
      font-weight: bold;
    }

    .styled-name {
      font-size: 40px;
      font-weight: 800;
      color: #2c3e50;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
      letter-spacing: 1.5px;
      background: linear-gradient(to right, #4a90e2, #00c6ff);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-bottom: 20px;
    }

    .social-links {
      margin-top: 10px;
    }

    .social-links a {
      margin: 0 10px;
      text-decoration: none;
      color: #4a90e2;
      font-weight: bold;
      font-size: 16px;
    }

    .social-links a:hover {
      color: #2c6fb2;
      text-decoration: underline;
    }

    .social-links i {
      margin-right: 6px;
      color: #4a90e2;
    }

    /* About Section */
    .about {
      background: #e6f2ff;
    }

    /* Contact Section */
    .contact {
      margin: 40px 20px;
      padding: 20px;
      background: #fff3cd;
      border-radius: 10px;
    }

    .contact h2 {
      color: #856404;
      margin-bottom: 15px;
    }

    .contact form {
      max-width: 400px;
      margin: 0 auto;
    }

    .contact input,
    .contact textarea {
      width: 100%;
      padding: 12px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 6px;
    }

    .contact button {
      background-color: #4a90e2;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }

    .contact button:hover {
      background-color: #2c6fb2;
    }

    /* Gallery Section */
    .gallery {
      margin: 40px 20px;
      background: #e8f0fe;
      padding: 20px;
      border-radius: 10px;
    }

    /* Responsive */
    @media (min-width: 600px) {
      .nav-links {
        flex-direction: row;
        position: static;
        background: none;
        display: flex !important;
      }

      .nav-links a {
        border: none;
        padding: 10px 15px;
        color: white;
      }

      .menu-icon {
        display: none;
      }
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <div class="navbar">
    <h2>Rihan's Portfolio</h2>
    <div class="menu-icon" onclick="toggleMenu()" aria-label="Toggle navigation menu">
      <div></div>
      <div></div>
      <div></div>
    </div>
    <div class="nav-links" id="navLinks">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
      <a href="#gallery">Gallery</a>
    </div>
  </div>

  <!-- Home Section -->
  <div class="section home" id="home">
    <h1 class="styled-name">Rakibul Hasan Rihan</h1>
    <div class="social-links">
      <a href="https://www.facebook.com/share/16iGimgYqJ/" target="_blank">
        <i class="fab fa-facebook"></i>Facebook
      </a>
      <a href="https://www.instagram.com/rakibul_hasan_12345" target="_blank">
        <i class="fab fa-instagram"></i>Instagram
      </a>
    </div>
  </div>

  <!-- About Section -->
  <div class="section about" id="about">
    <h2>About Me</h2>
    <p>
      Hello! I'm <strong>Rakibul Hasan Rihan</strong>, a passionate student and web enthusiast.
      I enjoy exploring the world of web development and creating simple, user-friendly websites.
      With basic HTML knowledge and growing interest in design, I'm building my digital portfolio step-by-step.
      This website represents my learning journey and a place where others can connect with me.
    </p>
  </div>

  <!-- Contact Section -->
  <div class="section contact" id="contact">
    <h2>Contact Me</h2>
    <form action="https://formsubmit.co/your@email.com" method="POST">
  <input type="text" name="name" placeholder="Your Name" required />
  <input type="email" name="email" placeholder="Your Email" required />
  <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
  <button type="submit">Send</button>
</form>
  </div>

  <!-- Gallery Section -->
  <div class="section gallery" id="gallery">
    <h2>Gallery</h2>
    <p>Gallery items will be shown here soon.</p>
  </div>

  <script>
    function toggleMenu() {
      document.getElementById("navLinks").classList.toggle("nav-active");
    }
  </script>

</body>
</html>