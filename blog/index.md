---
layout: default
title: Blogs
---

## ✍️ Blogs

<ul>
{% assign items = site.blog | sort: "date" | reverse %}
{% for item in items %}
  <li><a href="{{ item.url }}">{{ item.title }}</a> — {{ item.date | date: "%b %d, %Y" }}</li>
{% endfor %}
</ul>
