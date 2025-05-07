<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Souradeep Pradhan | Portfolio</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #0f0f0f;
      color: #f1f1f1;
      line-height: 1.6;
    }

    nav {
      background-color: #1f1f1f;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 4px 10px rgba(0,0,0,0.8);
    }

    nav h1 {
      font-size: 1.8em;
      color: #00bcd4;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 30px;
    }

    nav ul li a {
      text-decoration: none;
      color: #f1f1f1;
      font-weight: 500;
      transition: 0.3s;
    }

    nav ul li a:hover {
      color: #00bcd4;
    }

    header {
      text-align: center;
      padding: 60px 20px 40px;
      background: linear-gradient(145deg, #1a1a1a, #222);
    }

    header img {
      width: 160px;
      height: 160px;
      border-radius: 50%;
      object-fit: cover;
      border: 4px solid #00bcd4;
      box-shadow: 0 0 20px rgba(0,188,212,0.4);
      margin-bottom: 20px;
    }

    header h2 {
      font-size: 2.2em;
      color: #00bcd4;
      margin-bottom: 10px;
    }

    .container {
      max-width: 1100px;
      margin: 40px auto;
      padding: 40px;
      background: #1c1c1c;
      border-radius: 15px;
      box-shadow: 0 0 25px rgba(0,188,212,0.2);
    }

    .section {
      margin-bottom: 50px;
    }

    h3 {
      font-size: 1.8em;
      margin-bottom: 20px;
      border-left: 5px solid #00bcd4;
      padding-left: 15px;
    }

    .contact-links a {
      display: inline-block;
      background-color: #00bcd4;
      color: white;
      padding: 10px 25px;
      margin: 10px 15px 0 0;
      text-decoration: none;
      border-radius: 8px;
      font-weight: bold;
      transition: background 0.3s;
    }

    .contact-links a:hover {
      background-color: #0097a7;
    }

    ul {
      padding-left: 25px;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    input, textarea {
      padding: 12px;
      border: none;
      border-radius: 8px;
      background: #2a2a2a;
      color: #fff;
      font-size: 1em;
    }

    input[type="submit"] {
      background-color: #00bcd4;
      cursor: pointer;
      font-weight: bold;
      transition: background 0.3s;
    }

    input[type="submit"]:hover {
      background-color: #0097a7;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #111;
      color: #777;
      font-size: 14px;
    }
  </style>
</head>
<body>

<nav>
  <h1>Souradeep</h1>
  <ul>
    <li><a href="#about">Home</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<header>
  <img src="soura.webp" alt="Souradeep Pradhan">
  <h2>Souradeep Pradhan</h2>
  <p>B.Tech CSE Student | Creative Technophile</p>
</header>

<div class="container">
  <section class="section" id="about">
    <h3>About Me</h3>
    <p>Hello! I'm Souradeep, a Computer Science Engineering student from Adamas University, Kolkata. I'm passionate about tech, creativity, and innovation. I love coding, design, and producing content on YouTube to express my ideas and knowledge.</p>
  </section>

  <section class="section" id="skills">
    <h3>Skills & Certifications</h3>
    <ul>
      <li>Generative AI Fundamentals (Google Cloud Academy)</li>
      <!-- Add more skills here -->
    </ul>
  </section>

  <section class="section" id="projects">
    <h3>Projects</h3>
    <p>Coming Soon! I will showcase my best coding, design, and YouTube projects here.</p>
  </section>

  <section class="section" id="contact">
    <h3>Contact Me</h3>
    <form onsubmit="return validateEmail();">
      <input type="text" placeholder="Your Name" required>
      <input type="email" id="email" placeholder="Your Email" required>
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <input type="submit" value="Send Message">
    </form>
    <div class="contact-links">
      <a href="mailto:souradeeppradhan6@outlook.com">Email Me</a>
      <a href="https://www.linkedin.com/in/souradeep-pradhan-50b415329" target="_blank">LinkedIn</a>
      <a href="https://www.youtube.com/@Pradhan_Da" target="_blank">YouTube Subscribe Now </a>
    </div>
  </section>
</div>

<footer>
  &copy; 2025 Souradeep Pradhan. All rights reserved.
</footer>

<script>
  function validateEmail() {
    const email = document.getElementById("email").value;
    const pattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    if (!pattern.test(email)) {
      alert("Please enter a valid email address.");
      return false;
    }
    alert("Message sent successfully!");
    return true;
  }
</script>

</body>
</html>
