---
layout: default
title: Projects
permalink: /projects/
---

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
