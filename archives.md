---
layout: page
title: Old Blog Posts
---

<section>
  {% for post in site.posts %}
    _<a href="{{site.baseurl}}{{post.url}}"><strong>{{ post.title }}</strong></a>_
    <strong>{{ post.date | date: "%A, %B %e, %Y" }}</strong>
    <small>.<a class="category" href="{{site.baseurl}}/categories/{{ post.category | downcase }}.html">{{ post.category }}</a>.</small>
  {% endfor %}
</section>
