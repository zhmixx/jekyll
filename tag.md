---
layout: default
title: tags
permalink: /tag/
---

<ul>
  {% assign tags = site.tags | sort %}
  {% for tag in tags %}
    <li>
      <a href="/tag/{{ tag[0] | slugify }}/">{{ tag[0] }}</a> ({{ tag[1].size }})
    </li>
  {% endfor %}
</ul>
