---
layout: default
title: CTF Writeups
---

## 🧩 CTF Writeups

{% assign items = site.ctf | sort: "date" | reverse %}

**Total writeups found:** {{ items.size }}

{% if items.size == 0 %}
_No CTF writeups yet._
{% else %}
<ul>
{% for item in items %}
  <li>
    <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
    — {{ item.date | date: "%b %d, %Y" }}
  </li>
{% endfor %}
</ul>
{% endif %}
