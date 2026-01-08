---
title: Blogs
---

# ✍️ Blogs

{% assign items = site.blog | sort: "date" | reverse %}

{% if items.size == 0 %}
No blog posts yet. Add your first post in <code>_blog/</code>.
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
