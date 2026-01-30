---
layout: default
title: Projects
permalink: /projects/
---

<div class="nav-container">
  <a href="{{ '/' | relative_url }}" class="nav-link">🏠 Home</a>
  <a href="{{ '/blog' | relative_url }}" class="nav-link">📰 Blog</a>
  <a href="{{ '/projects' | relative_url }}" class="nav-link" style="background-color: #0366d6; color: white;">💻 Projects</a>
</div>

# 💻 My Projects

<div class="grid-container">
  {% for project in site.data.projects %}
  <a href="{{ project.url }}" class="card" target="_blank">
    <div class="card-title">{{ project.title }}</div>
    <div class="card-desc">{{ project.description }}</div>
    <div class="card-tags">
      {% for tag in project.tags %}
      <span class="tag">{{ tag }}</span>
      {% endfor %}
    </div>
  </a>
  {% endfor %}
</div>
