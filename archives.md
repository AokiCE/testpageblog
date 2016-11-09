---
layout: page
title: Old Blog Posts
---

<section>
<h4 align="left">
  <strong>{{ post.date | date_to_string }}</strong>
    <small>.
    <a class="category" href="{{site.baseurl}}/categories/{{ post.category | downcase }}.html">
      {{ post.category }}
    </a>
  .</small>
  <br class="visible-xs-block">
  <a href="{{site.baseurl}}{{post.url}}">
    <strong>{{ post.title }}</strong>
  </a>

</h4>
</section>
    
{% include pagination.html %}
