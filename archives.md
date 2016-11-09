---
layout: page
title: Old Blog Posts
---

<section>
  {% for post in site.posts %}
  <strong>{{ post.date | date: "%A, %B %e, %Y" }}</strong>
    <small>.
    <a class="category" href="{{site.baseurl}}/categories/{{ post.category | downcase }}.html">
      {{ post.category }}
    </a>
  .</small>
  <br class="visible-xs-block">
  <a href="{{site.baseurl}}{{post.url}}">
    <strong>{{ post.title }}</strong>
  </a>
  {% endfor %}
</section>
