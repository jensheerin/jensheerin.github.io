
---
layout: default
title: Home
---

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,initial-scale=1.0">
  <title>{{ site.title }} - Home</title>
  <link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">
</head>
<body>
  <header>
    <h1>{{ site.title }}</h1>
    <p>{{ site.description }}</p>
    <nav>
      <a href="{{ '/' | relative_url }}">Home</a>
      <a href="{{ '/about/' | relative_url }}">About</a>
      <a href="{{ '/blog/' | relative_url }}">Blog</a>
    </nav>
  </header>
  <main>
    <section>
      <h2>Welcome to My Blog!</h2>
      <p>This is the home page for {{ site.title }}. Here you'll find my latest posts, thoughts, and updates.</p>
    </section>
    <section>
      <h2>Recent Posts</h2>
      <ul>
        {% for post in site.posts limit:5 %}
          <li>
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
            <span>{{ post.date | date: "%B %d, %Y" }}</span>
          </li>
        {% endfor %}
      </ul>
      <a href="{{ '/blog/' | relative_url }}">See all posts &rarr;</a>
    </section>
  </main>
  <footer>
    <p>&copy; {{ site.time | date: "%Y" }} {{ site.title }}. Powered by <a href="https://jekyllrb.com/">Jekyll</a>.</p>
  </footer>
</body>
</html>
