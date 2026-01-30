---
layout: default
title: Blog
permalink: /blog/
---

<div class="nav-container">
  <a href="{{ '/' | relative_url }}" class="nav-link">🏠 Home</a>
  <a href="{{ '/blog' | relative_url }}" class="nav-link" style="background-color: #0366d6; color: white;">📰 Blog</a>
  <a href="{{ '/projects' | relative_url }}" class="nav-link">💻 Projects</a>
</div>

# 📰 Blog Posts

<div class="grid-container">
  {% for post in site.posts %}
  <a href="{{ post.url | relative_url }}" class="card">
    <div class="card-title">{{ post.title }}</div>
    <div class="card-desc">{{ post.description }}</div>
    <div class="card-tags">
      <span class="tag">{{ post.date | date: "%B %d, %Y" }}</span>
    </div>
  </a>
  {% endfor %}
</div>
