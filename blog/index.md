---
layout: default
title: Blogs
---

# ✍️ Blogs

<ul>
  {% for post in site.categories.blog %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%b %d, %Y" }}</li>
  {% endfor %}
</ul>
