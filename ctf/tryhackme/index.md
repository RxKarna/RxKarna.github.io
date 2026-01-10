---
title: TryHackMe Writeups
---

# 🎯 TryHackMe Writeups

{% assign items = site.ctf | where_exp: "p", "p.path contains 'tryhackme/'" %}
{% if items.size == 0 %}
No writeups yet.
{% else %}
{% for post in items %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %d, %Y" }}
{% endfor %}
{% endif %}
