---
layout: default
title: Home
---

## ./ RxKarna
*Cybersecurity Researcher | Pentesting | CTF Writeups | Security Notes*

> I document hands-on security learning: *CTF writeups, **practical notes, and **blogs/research* — written clearly for beginners and useful for experienced folks.

[🧩 CTF Writeups](/ctf/) • [📒 Notes](/notes/) • [✍️ Blogs](/blog/)  
[GitHub](https://github.com/RxKarna)

---

## What you’ll find here

<table>
<tr>
<td width="33%">

### 🧩 CTF Writeups
Walkthroughs with recon → exploitation → privilege escalation → lessons learned.  
*Goal:* show methodology and thinking.

[Open CTF →](/ctf/)

</td>
<td width="33%">

### 📒 Cybersecurity Notes
Cheatsheets, commands, concepts, and quick references.  
*Goal:* fast recall + structured learning.

[Open Notes →](/notes/)

</td>
<td width="33%">

### ✍️ Blogs
Longer posts: research, opinions, breakdowns, and tools.  
*Goal:* deeper understanding.

[Open Blogs →](/blog/)

</td>
</tr>
</table>

---

## ⭐ Featured (Best to start with)

- *[First CTF Writeup – Example](/ctf/first-ctf-writeup-example/)* — CTF  
- *[Nmap Cheatsheet – Example](/notes/nmap-cheatsheet-example/)* — Notes  
- *[Why I Like CTFs](/blog/why-i-like-ctfs/)* — Blog  

---

## 🔥 Latest updates

<table>
<tr>
<td width="33%">

### 🧩 Latest CTF
{% assign ctf_items = site.ctf | sort: "date" | reverse | slice: 0, 5 %}
{% if ctf_items.size == 0 %}
No CTF writeups yet.
{% else %}
<ul>
{% for item in ctf_items %}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a><br><small>{{ item.date | date: "%b %d, %Y" }}</small></li>
{% endfor %}
</ul>
{% endif %}

</td>
<td width="33%">

### 📒 Latest Notes
{% assign note_items = site.notes | sort: "date" | reverse | slice: 0, 5 %}
{% if note_items.size == 0 %}
No notes yet.
{% else %}
<ul>
{% for item in note_items %}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a><br><small>{{ item.date | date: "%b %d, %Y" }}</small></li>
{% endfor %}
</ul>
{% endif %}

</td>
<td width="33%">

### ✍️ Latest Blogs
{% assign blog_items = site.blog | sort: "date" | reverse | slice: 0, 5 %}
{% if blog_items.size == 0 %}
No blog posts yet.
{% else %}
<ul>
{% for item in blog_items %}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a><br><small>{{ item.date | date: "%b %d, %Y" }}</small></li>
{% endfor %}
</ul>
{% endif %}

</td>
</tr>
</table>

---

## 🔎 Quick Search
Search everything using Google:  
site:rxkarna.github.io <keyword>
