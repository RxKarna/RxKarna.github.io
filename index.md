---
layout: default
title: Home
---

Practical cybersecurity learning — clearly documented, reproducible, and beginner-friendly.

[🧩 Explore CTF →](/ctf/) • [📒 Explore Notes →](/notes/) • [✍️ Explore Blogs →](/blog/)

---

## What you’ll find here

### 🧩 CTF Writeups
- Recon → Exploitation → PrivEsc
- Commands used + reasoning + lessons learned
- Written to be reproducible

### 📒 Cybersecurity Notes
- Cheatsheets & quick references
- Concepts explained simply
- Useful for daily practice

### ✍️ Blogs
- Longer posts: research, breakdowns, opinions
- Tool walkthroughs
- Learning journeys

---

## ⭐ Featured (Start here)
- 🧩 **First CTF Writeup — Example** → [Open](/ctf/first-ctf-writeup/)
- 📒 **Nmap Cheatsheet — Example** → [Open](/notes/nmap-cheatsheet/)
- ✍️ **Why I Like CTFs** → [Open](/blog/why-i-like-ctfs/)

---

## 🔥 Recent Activity

### 🧩 Latest CTF
<ul>
{% assign items = site.ctf | sort: "date" | reverse %}
{% for item in items limit:5 %}
  <li><a href="{{ item.url }}">{{ item.title }}</a> — {{ item.date | date: "%b %d, %Y" }}</li>
{% endfor %}
</ul>

### 📒 Latest Notes
<ul>
{% assign items = site.notes | sort: "date" | reverse %}
{% for item in items limit:5 %}
  <li><a href="{{ item.url }}">{{ item.title }}</a> — {{ item.date | date: "%b %d, %Y" }}</li>
{% endfor %}
</ul>

### ✍️ Latest Blogs
<ul>
{% assign items = site.blog | sort: "date" | reverse %}
{% for item in items limit:5 %}
  <li><a href="{{ item.url }}">{{ item.title }}</a> — {{ item.date | date: "%b %d, %Y" }}</li>
{% endfor %}
</ul>

---

## Why this site exists
This is my public learning archive. Everything here is hands-on, reproducible, and written while learning — not copied.
