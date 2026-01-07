---
layout: default
title: Home
---

# ./ RxKarna

Welcome 👋  
This site is my personal space for *CTF writeups, cybersecurity notes, and blog posts*.

---

## 📌 Sections

- *CTF Writeups* → [Open](/ctf/)
- *Cybersecurity Notes* → [Open](/notes/)
- *Blogs* → [Open](/blog/)

---

## 🔥 Latest Posts

### CTF Writeups
<ul>
  {% for post in site.categories.ctf limit:5 %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%b %d, %Y" }}</li>
  {% endfor %}
</ul>

### Cybersecurity Notes
<ul>
  {% for post in site.categories.notes limit:5 %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%b %d, %Y" }}</li>
  {% endfor %}
</ul>

### Blogs
<ul>
  {% for post in site.categories.blog limit:5 %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%b %d, %Y" }}</li>
  {% endfor %}
</ul>
