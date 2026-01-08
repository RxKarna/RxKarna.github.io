---
title: Cybersecurity Notes
---

# 📒 Cybersecurity Notes

{% assign items = site.notes | sort: "date" | reverse %}

{% if items.size == 0 %}
No notes yet. Add your first note in <code>_notes/</code>.
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
