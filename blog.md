---
layout: page
title: Blog
permalink: /blog/
---

# Blog

Welcome to the blog! Here are the latest posts:

<ul>
  {% for post in site.posts %}
    <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%b %-d, %Y" }}</li>
  {% endfor %}
</ul>

**Debug Info**

- `site.baseurl`: `{{ site.baseurl }}`
- `post.url`: `{{ site.posts[0].url }}`
- `Final link`: `{{ site.baseurl }}{{ site.posts[0].url }}`
