---
title: Blogs
---

# ✍️ Blogs

{% if site.blogs.size == 0 %}
No blogs yet.
{% else %}
{% for post in site.blogs %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %d, %Y" }}
{% endfor %}
{% endif %}
