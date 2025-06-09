<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Rihan's Portfolio</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #f4f4f4;
    }

    /* Navbar */
    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: #222;
      color: white;
      padding: 15px 20px;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 1000;
    }

    .navbar h2 {
      margin: 0;
      font-size: 20px;
    }

    .menu-icon {
      cursor: pointer;
      width: 30px;
    }

    .menu-icon div {
      height: 4px;
      background-color: white;
      margin: 5px 0;
      border-radius: 2px;
    }

    .nav-links {
      display: none;
      flex-direction: column;
      background-color: #333;
      position: absolute;
      top: 60px;
      left: 0;
      width: 100%;
    }

    .nav-links a {
      color: white;
      padding: 15px 20px;
      text-decoration: none;
      border-top: 1px solid #444;
    }

    .nav-links a:hover {
      background-color: #444;
    }

    .nav-active {
      display: flex;
    }

    .main-content {
      padding: 100px 20px 40px;
      text-align: center;
    }

    /* Gallery Section */
    .gallery {
      margin-top: 40px;
    }

    .gallery h2 {
      font-size: 24px;
      margin-bottom: 20px;
    }

    .gallery p {
      color: #555;
    }

    /* Contact Section */
    .contact {
      padding: 40px 20px;
      background-color: #fff;
      margin-top: 40px;
    }

    .contact h2 {
      margin-bottom: 20px;
    }

    .contact form {
      max-width: 400px;
      margin: 0 auto;
    }

    .contact input,
    .contact textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    .contact button {
      background-color: #222;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }

    .contact button:hover {
      background-color: #444;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <div class="navbar">
    <h2>Rihan's Site</h2>
    <div class="menu-icon" onclick="toggleMenu()">
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>

  <!-- Menu -->
  <div class="nav-links" id="navLinks">
    <a href="#contact">Contact</a>
    <a href="#gallery">Gallery</a>
  </div>

  <!-- Main Content -->
  <div class="main-content">
    <h1>Welcome to My Website</h1>
    <p>This is a simple portfolio website created by Rakibul Hasan Rihan.</p>
  </div>

  <!-- Gallery Section -->
  <div class="gallery" id="gallery">
    <h2>Gallery</h2>
    <p>Gallery content coming soon...</p>
  </div>

  <!-- Contact Section -->
  <div class="contact" id="contact">
    <h2>Contact Me</h2>
    <form action="mailto:rhr6263@gmail.com" method="post" enctype="text/plain">
      <input type="text" name="name" placeholder="Your Name" required />
      <input type="email" name="email" placeholder="Your Email" required />
      <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </div>

  <script>
    function toggleMenu() {
      document.getElementById("navLinks").classList.toggle("nav-active");
    }
  </script>

</body>
</html>