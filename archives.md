---
layout: page
title: Old Blog Posts
---

<section>
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
</section>
