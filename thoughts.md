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
      
      {%- if post.external_url -%}
        <h3><a href="{{ post.external_url }}" target="_blank" rel="noopener noreferrer">{{ post.title }} ↗</a></h3>
      {%- else -%}
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      {%- endif -%}

      <p><em>{{ post.date | date_to_string }}</em></p>
      <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
    </li>
  {% endfor %}
</ul>