---
layout: default
title: CTF Writeups
---

## 🧩 CTF Writeups

<ul>
{% assign items = site.ctf | sort: "date" | reverse %}
{% for item in items %}
  <li><a href="{{ item.url }}">{{ item.title }}</a> — {{ item.date | date: "%b %d, %Y" }}</li>
{% endfor %}
</ul>
