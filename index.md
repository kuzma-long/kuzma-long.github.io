---
layout: home
title: 首页
---

<div class="home-archive">
  {% for post in site.posts %}
  <article>
    <a href="{{ post.url | relative_url }}">
      <h2>{{ post.title }}</h2>
      <p>{{ post.excerpt | strip_html | truncate: 100 }}</p>
    </a>
  </article>
  {% endfor %}
</div>
