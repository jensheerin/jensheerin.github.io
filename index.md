---
layout: default
title: About Me
---

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,initial-scale=1.0">
  <title>{{ site.title }} - Jen Sheerin</title>
  <link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">
  <style>
    body {
      font-family: 'Segoe UI', 'Roboto', Arial, sans-serif;
      background: linear-gradient(120deg, #e0eafc 0%, #cfdef3 100%);
      margin: 0;
      padding: 0;
    }
    .about-container {
      max-width: 800px;
      margin: 40px auto;
      background: #fff;
      border-radius: 16px;
      box-shadow: 0 4px 24px rgba(0,0,0,0.07);
      padding: 40px 32px;
      animation: fadeIn 1s;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px);}
      to { opacity: 1; transform: translateY(0);}
    }
    .profile-img {
      width: 140px;
      height: 140px;
      object-fit: cover;
      border-radius: 50%;
      box-shadow: 0 4px 18px rgba(0,0,0,0.09);
      margin-bottom: 24px;
      border: 4px solid #e0eafc;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
    h1 {
      text-align: center;
      font-size: 2.6em;
      margin-bottom: 10px;
      color: #2a5298;
      font-weight: 700;
    }
    h2 {
      color: #4169e1;
      margin-top: 30px;
      font-size: 1.4em;
      border-bottom: 1px solid #e0eafc;
      padding-bottom: 5px;
      margin-bottom: 18px;
    }
    .about-content {
      font-size: 1.17em;
      line-height: 1.7;
      color: #333;
      text-align: center;
      margin-bottom: 12px;
    }
    .about-details {
      margin-top: 36px;
      display: flex;
      flex-wrap: wrap;
      gap: 32px;
      justify-content: center;
    }
    .detail-card {
      background: #f6faff;
      border-radius: 10px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.04);
      padding: 24px 18px;
      min-width: 220px;
      max-width: 280px;
      text-align: left;
      flex: 1 1 220px;
    }
    .detail-card h3 {
      margin-top: 0;
      color: #2a5298;
      font-size: 1.1em;
      margin-bottom: 6px;
    }
    .social-links {
      margin-top: 32px;
      text-align: center;
    }
    .social-links a {
      display: inline-block;
      margin: 0 9px;
      color: #4169e1;
      font-size: 1.5em;
      transition: color 0.2s;
    }
    .social-links a:hover {
      color: #2a5298;
      text-decoration: none;
    }
    @media (max-width: 600px) {
      .about-container { padding: 18px; }
      .about-details { flex-direction: column; gap: 16px; }
    }
  </style>
</head>
<body>
  <header>
    <nav style="text-align:center; margin-top:18px;">
      <a href="{{ '/' | relative_url }}">Home</a>
      <a href="{{ '/about/' | relative_url }}" style="font-weight:bold;">About</a>
      <a href="{{ '/blog/' | relative_url }}">Blog</a>
    </nav>
  </header>
  <main>
    <div class="about-container">
      <!-- Replace the src below with your own photo if available -->
      <img src="https://avatars.githubusercontent.com/{{ site.github.owner }}" alt="Profile photo" class="profile-img">
      <h1>Hi, I'm {{ site.title }}</h1>
      <div class="about-content">
        <p>
          Welcome to my personal page! I'm passionate about technology, code, and continuous learning.
          Here you'll find more about my journey, skills, and interests.
        </p>
      </div>
      <div class="about-details">
        <div class="detail-card">
          <h3>👨‍💻 What I Do</h3>
          <p>
            Senior Cloud & AI Solution Engineer and tech enthusiast. I experiment with new AI technologies.
          </p>
        </div>
        <div class="detail-card">
        </div>
        <div class="detail-card">
          <h3>🎯 Interests</h3>
          <p>
            AI & ML, DevOps, DevSecOps, open source, blogging, design, and exploring new tech trends and tools.
          </p>
        </div>
        <div class="detail-card">
          <h3>🌎 Location</h3>
          <p>
           Love remote work and global collaboration!
          </p>
        </div>
      </div>
      <section class="social-links">
        <a href="https://github.com/{{ site.github.owner }}" title="GitHub" target="_blank"><i class="fab fa-github"></i>🐙</a>
        <!-- Add more social links as needed -->
      </section>
    </div>
  </main>
  <footer style="text-align:center; margin-top:38px;">
    <p>&copy; {{ site.time | date: "%Y" }} {{ site.title }}. Powered by <a href="https://jekyllrb.com/">Jekyll</a>.</p>
  </footer>
</body>
</html>
