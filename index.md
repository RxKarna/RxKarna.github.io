---
title: Home
---

# ./ RxKarna — Cybersecurity Researcher

Practical cybersecurity learning — clearly documented, reproducible, and beginner-friendly.

- 🧩 [Explore CTF →](/ctf/)
- 📒 [Explore Notes →](/notes/)
- ✍️ [Explore Blogs →](/blog/)

---

## What you’ll find here

### 🧩 CTF Writeups
Recon → Exploitation → PrivEsc → Lessons learned, with commands and reasoning.

### 📒 Cybersecurity Notes
Cheatsheets, commands, and concepts explained simply.

### ✍️ Blogs
Longer posts: research, tool breakdowns, and learning journeys.

---

## ⭐ Featured (Best to start with)

### 🧩 Latest CTF
{% assign items = site.ctf | sort: "date" | reverse %}
{% for item in items limit: 3 %}
- [{{ item.title }}]({{ item.url }}){% if item.date %} — {{ item.date | date: "%b %d, %Y" }}{% endif %}
{% endfor %}

### 📒 Latest Notes
{% assign items = site.notes | sort: "date" | reverse %}
{% for item in items limit: 3 %}
- [{{ item.title }}]({{ item.url }}){% if item.date %} — {{ item.date | date: "%b %d, %Y" }}{% endif %}
{% endfor %}

### ✍️ Latest Blogs
{% assign items = site.blog | sort: "date" | reverse %}
{% for item in items limit: 3 %}
- [{{ item.title }}]({{ item.url }}){% if item.date %} — {{ item.date | date: "%b %d, %Y" }}{% endif %}
{% endfor %}
