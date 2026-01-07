---
layout: default
title: CTF Writeups
---

# 🧩 CTF Writeups

<ul>
{% assign items = site.ctf | reverse %}
{% for item in items %}
  <li><a href="{{ item.url }}">{{ item.title }}</a></li>
{% endfor %}
</ul>
