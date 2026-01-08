---
layout: default
title: Cybersecurity Notes
---

## 📒 Cybersecurity Notes

<ul>
{% assign items = site.notes | sort: "date" | reverse %}
{% for item in items %}
  <li><a href="{{ item.url }}">{{ item.title }}</a> — {{ item.date | date: "%b %d, %Y" }}</li>
{% endfor %}
</ul>
