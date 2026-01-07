---
layout: default
title: Cybersecurity Notes
---

## 📒 Cybersecurity Notes

{% assign items = site.notes | sort: "date" | reverse %}

**Total notes found:** {{ items.size }}

{% if items.size == 0 %}
_No notes yet._
{% else %}
<ul>
{% for item in items %}
  <li>
    <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
    {% if item.date %}— {{ item.date | date: "%b %d, %Y" }}{% endif %}
  </li>
{% endfor %}
</ul>
{% endif %}
