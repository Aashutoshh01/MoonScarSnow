---
layout: default
title: Blog
permalink: /blog/
---

<h1 data-aos="fade-right">📰 Blog Posts</h1>

<div class="grid-container">
  {% for post in site.posts %}
  <a href="{{ post.url | relative_url }}" class="card tilt-card" data-aos="fade-up" data-aos-delay="{{ forloop.index0 | times: 100 }}">
    <div class="tilt-card-inner">
      <div class="card-title">{{ post.title }}</div>
      <div class="card-desc">{{ post.description }}</div>
      <div class="card-tags">
        <span class="tag">{{ post.date | date: "%B %d, %Y" }}</span>
      </div>
    </div>
  </a>
  {% endfor %}
</div>
