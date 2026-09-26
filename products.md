---
layout: default
title: "My Apps & Projects"
permalink: /products/
---

## Apps & Projects

<span style="display: block; text-align: right; font-size: 14px; font-weight: bold; font-style: italic;">
    (Also, <a href="https://nextfive.xyz/library" target="_blank" style="font-size: inherit; font-weight: inherit; font-style: inherit; color: var(--nav-link-color);"> some small utilities and games </a> I'd fun creating) 
</span>

<ul class="post-list">
  {% for post in site.categories.product %}
    <li>
      <a href="{{ post.url | relative_url }}" class="post-card">
        <div class="post-card-header">
          <h3>{{ post.title }}</h3>
          <span class="post-card-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        </div>
        
        <p class="post-card-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
        
        <div class="post-card-footer">
          <span class="post-card-meta">{{ post.content | number_of_words }} words</span>
          <span class="read-more">Read more</span>
        </div>
      </a>
    </li>
  {% endfor %}
</ul>
