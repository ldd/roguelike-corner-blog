---
layout: default
---

<div class="blog-post-header"></div>

<div class="blog-post-content">
  {{ content }}
</div>
{% assign post = page %} 
{% include formatted_date.md %}
{% include comments.md %}
