---
layout: default
title: Home
---

# ./ RxKarna

Welcome 👋  
This site is my personal space for *CTF writeups, cybersecurity notes, and blog posts*.

---

## 📌 Collections

- *CTF Writeups* → [Open](/ctf/)
- *Cybersecurity Notes* → [Open](/notes/)
- *Blogs* → [Open](/blog/)

---

## 🔥 Latest Posts

### 🧩 CTF Writeups
<ul>
{% assign items = site.ctf | reverse %}
{% for item in items limit:5 %}
  <li><a href="{{ item.url }}">{{ item.title }}</a></li>
{% endfor %}
</ul>

### 📒 Cybersecurity Notes
<ul>
{% assign items = site.notes | reverse %}
{% for item in items limit:5 %}
  <li><a href="{{ item.url }}">{{ item.title }}</a></li>
{% endfor %}
</ul>

### ✍️ Blogs
<ul>
{% assign items = site.blog | reverse %}
{% for item in items limit:5 %}
  <li><a href="{{ item.url }}">{{ item.title }}</a></li>
{% endfor %}
</ul>
