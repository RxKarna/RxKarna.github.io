---
layout: default
title: Blogs
---

## ✍️ Blogs

{% assign items = site.blog | sort: "date" | reverse %}

**Total blog posts found:** {{ items.size }}

{% if items.size == 0 %}
_No blog posts yet._
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
