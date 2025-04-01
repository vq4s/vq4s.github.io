---
layout: default
title: Blog
permalink: /blog/
---

<div class="posts">
  {% for post in site.posts %}
  <article class="post">
    <h1 class="post-title">
      <a href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
    </h1>

    <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
    
    <a href="{{ post.url | relative_url }}">Read more →</a>
  </article>
  <hr>
  {% endfor %}
</div>
