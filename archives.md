---
layout: page
title: Archive of Blog Posts
---

<section>
<ul>
  {% for post in site.posts %}
  <li>
  <i><a href="{{site.baseurl}}{{post.url}}"><h2><strong>{{ post.title }}</strong></h2></a></i> --- <h4><strong>{{ post.date | date: "%B %e, %Y" }}</strong></h4>
<h5><a class="category" href="{{site.baseurl}}/categories/{{ post.category | downcase }}.html">{{ post.category }}</a></h5>
  </li>
  {% endfor %}
</ul>
</section>
