---
layout: default
title: Blog
permalink: /blog/
---

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
