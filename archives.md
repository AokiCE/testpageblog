---
layout: page
title: Archive of Blog Posts
---

<section>

  {% for post in site.posts %}

  * <i><a href="{{site.baseurl}}{{post.url}}"> **{{ post.title }}** </a></i> --- {{ post.date | date: "%B %e, %Y" }} 
  <a class="category" href="{{site.baseurl}}/categories/{{ post.category | downcase }}.html">{{ post.category }}</a>

  {% endfor %}

</section>
