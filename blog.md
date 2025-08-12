---
layout: default
title: "Blog"
permalink: /blog/
---
## Blog
<ul>
  {% for post in site.categories.musings %}
    <li><h3><a href="{{ post.url }}">{{ post.title }}</a></h3><p><em>{{ post.date | date_to_string }}</em></p><p>{{ post.excerpt }}</p></li>
  {% endfor %}
</ul>
