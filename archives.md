---
layout: page
title: Old Blog Posts
---

<section>
<ul>
  {% for post in site.posts %}
  <li>
    <i><a href="{{site.baseurl}}{{post.url}}"><strong>{{ post.title }}</strong></a></i>
    <strong>{{ post.date | date: "%A, %B %e, %Y" }}</strong>
    <small>.<a class="category" href="{{site.baseurl}}/categories/{{ post.category | downcase }}.html">{{ post.category }}</a>.</small>
  </li>
  {% endfor %}
</ul>
</section>
