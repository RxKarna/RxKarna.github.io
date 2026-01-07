---
layout: default
title: CTF Writeups
---

# 🧩 CTF Writeups

<ul>
  {% for post in site.categories.ctf %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%b %d, %Y" }}</li>
  {% endfor %}
</ul>
