---
layout: default
title: Blogs
---

# ✍️ Blogs

<ul>
{% assign items = site.blog | reverse %}
{% for item in items %}
  <li><a href="{{ item.url }}">{{ item.title }}</a></li>
{% endfor %}
</ul>
