---
layout: default
title: Home
---
A personal archive of cybersecurity research and CTF writeups.

---

## 📌 Collections
- **CTF Writeups** → [Open](/ctf/)
- **Cybersecurity Notes** → [Open](/notes/)
- **Blogs** → [Open](/blog/)

---

## 🔥 Latest Posts

### 🧩 CTF Writeups
{% assign ctf_items = site.ctf | sort: "date" | reverse | slice: 0, 5 %}
{% if ctf_items.size == 0 %}
_No CTF writeups yet._
{% else %}
<ul>
{% for item in ctf_items %}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a> — {{ item.date | date: "%b %d, %Y" }}</li>
{% endfor %}
</ul>
{% endif %}

### 📒 Cybersecurity Notes
{% assign note_items = site.notes | sort: "date" | reverse | slice: 0, 5 %}
{% if note_items.size == 0 %}
_No notes yet._
{% else %}
<ul>
{% for item in note_items %}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a>{% if item.date %} — {{ item.date | date: "%b %d, %Y" }}{% endif %}</li>
{% endfor %}
</ul>
{% endif %}

### ✍️ Blogs
{% assign blog_items = site.blog | sort: "date" | reverse | slice: 0, 5 %}
{% if blog_items.size == 0 %}
_No blog posts yet._
{% else %}
<ul>
{% for item in blog_items %}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a> — {{ item.date | date: "%b %d, %Y" }}</li>
{% endfor %}
</ul>
{% endif %}
