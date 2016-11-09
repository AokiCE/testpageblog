---
layout: page
title: Archive of Blog Posts
---

<section>
<ul>
  {% for post in site.posts %}
  <li>
  <h3><i><a href="{{site.baseurl}}{{post.url}}"><strong>{{ post.title }}</strong></a></i> --- <strong>{{ post.date | date: "%B %e, %Y" }}</strong> <small><a class="category" href="{{site.baseurl}}/categories/{{ post.category | downcase }}.html">{{ post.category }}</a></small></h3>
  </li>
  {% endfor %}
</ul>
</section>
