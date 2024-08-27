---
layout: default
title: mes posts
permalink: /mesposts/
---

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h3>
        <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h3>
      <p class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</p>
      <p>{{ post.excerpt | escape }}</p>
    </li>
  {% endfor %}
</ul>
