---
title: Other CTFs
---

# 🌍 Other CTFs

{% assign items = site.ctf | where_exp: "p", "p.path contains 'other/'" %}
{% if items.size == 0 %}
No writeups yet.
{% else %}
{% for post in items %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %d, %Y" }}
{% endfor %}
{% endif %}
