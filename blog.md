---
layout: home
title: Blog
permalink: /blog/
---

# Blog

Welcome to the blog! Here are the latest posts:

<ul>
  {% for post in site.posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%b %-d, %Y" }}</li>
  {% endfor %}
</ul>
