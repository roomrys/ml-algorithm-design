---
layout: page
title: Weekly Plans
permalink: /weeklies/
---

# Weekly Plans

<ul>
{% assign weeks = site.pages | where_exp:"page","page.path contains 'weeklies/week'" | sort: "path" %}
{% for week in weeks %}
  <li><a href="{{ site.baseurl }}{{ week.url }}">{{ week.title | default: week.name }}</a></li>
{% endfor %}
</ul>
