---
layout: default
title: categories
permalink: /category/
---

<ul>
  {% assign categories = site.categories | sort %}
  {% for category in categories %}
    <li>
      <a href="/category/{{ category[0] | slugify }}/">{{ category[0] }}</a> ({{ category[1].size }})
    </li>
  {% endfor %}
</ul>
