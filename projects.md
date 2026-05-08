---
layout: default
title: Projects
permalink: /projects/
---

<h1 data-aos="zoom-out-up">💻 My Projects</h1>

<div class="grid-container">
  {% for project in site.data.projects %}
  <a href="{{ project.url }}" class="card tilt-card" target="_blank" data-aos="flip-left" data-aos-delay="{{ forloop.index0 | times: 100 }}">
    <div class="tilt-card-inner">
      <div class="card-title">{{ project.title }}</div>
      <div class="card-desc">{{ project.description }}</div>
      <div class="card-tags">
        {% for tag in project.tags %}
        <span class="tag">{{ tag }}</span>
        {% endfor %}
      </div>
    </div>
  </a>
  {% endfor %}
</div>
