---
title: CTF Writeups
---

# 🧩 CTF Writeups

{% assign items = site.ctf | sort: "date" | reverse %}

{% if items.size == 0 %}
No CTF writeups yet.
{% else %}
<ul>
  {% for item in items %}
    <li>
      <a href="{{ item.url }}">{{ item.title }}</a>
      {% if item.date %} — {{ item.date | date: "%b %d, %Y" }}{% endif %}
    </li>
  {% endfor %}
</ul>
{% endif %}
