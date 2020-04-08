---
layout: default
title: Tutorials & Tips Blog
---

<div class="panel">
  <div class="panel-body">
{% for post in site.posts %}

  <div class="tile">
    <div class="tile-content">
      <a href="{{ post.url | relative_url }}">
      <h2 class="blog-post-title tile-title">{{ post.title }}</h2>
      </a>
      {% include formatted_date.md %}
      {% for tag in post.tags %}
      <span class="label">{{ tag }}</span>
      {% endfor %}
      <p class="tile-subtitle">{{ post.excerpt }}</p>
    </div>

  </div>
{% endfor %}
  </div>
</div>
