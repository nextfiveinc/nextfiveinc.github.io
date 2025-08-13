---
layout: default
title: "Thoughts"
permalink: /thoughts/
---
## Thoughts

My thoughts on software, design, and simplicity.

<ul>
  {% for post in site.categories.blog %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p><em>{{ post.date | date_to_string }}</em></p>
      <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
    </li>
  {% endfor %}
</ul>
