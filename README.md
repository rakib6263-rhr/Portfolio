<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Rakibul Hasan Rihan - Portfolio</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f4;
      color: #333;
    }
    header {
      background-color: #0d47a1;
      color: white;
      padding: 20px;
      text-align: center;
    }
    .social-icons a {
      margin: 0 10px;
      color: white;
      text-decoration: none;
      font-size: 20px;
    }
    section {
      padding: 20px;
      max-width: 600px;
      margin: auto;
      background: white;
      border-radius: 10px;
      margin-top: 30px;
    }
    form {
      display: flex;
      flex-direction: column;
    }
    input, textarea {
      padding: 10px;
      margin-bottom: 15px;
      border-radius: 8px;
      border: 1px solid #ccc;
      font-size: 1rem;
    }
    button {
      padding: 10px;
      background-color: #3b82f6;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 1rem;
      cursor: pointer;
    }
    button:hover {
      background-color: #2563eb;
    }
  </style>
</head>
<body>

<header>
  <h1>Rakibul Hasan Rihan</h1>
  <p>I'm a Student & Web Enthusiast</p>
  <img src="rihan.png" alt="My Photo" style="width: 200px; border-radius: 50%; margin-top: 20px;" />
  <div class="social-icons">
    <a href="https://www.facebook.com/share/16iGimgYqJ/" target="_blank">Facebook</a>
    <a href="https://www.instagram.com/rakibul_hasan_12345?igsh=eWV0cmRhb3d6YWFl" target="_blank">Instagram</a>
  </div>
</header>
<section>
  <h2>About Me</h2>
  <p>
    Hi! I'm Rakibul Hasan Rihan. I'm a student who loves learning about web design and development.
    I know a bit of HTML and enjoy building simple websites. My goal is to improve my skills and
    create more professional-looking websites like this portfolio!
  </p>
</section>
<section>
  <h2>Contact Me</h2>
  <form action="https://formsubmit.co/rhr6263@gmail.com" method="POST">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>

    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="5" required></textarea>

    <button type="submit">Send Message</button>
  </form>
</section>

</body>
</html>
