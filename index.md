---
layout: default
title: "Next Five Things"
---
## Latest Writings
<ul>
  {% for post in site.posts %}
    <li>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p><em>{{ post.date | date_to_string }}</em></p>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
