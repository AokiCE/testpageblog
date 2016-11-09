---
layout: page
title: Archive of Blog Posts
---

<section>

  {% for post in site.posts %}
<ul>
  <li>
    <p>
    <h2><i><a href="{{site.baseurl}}{{post.url}}"><strong>{{ post.title }}</strong></a></i></h2> --- {{ post.date | date: "%B %e, %Y" }} 
    <a class="category" href="{{site.baseurl}}/categories/{{ post.category | downcase }}.html"><i>{{ post.category }}</i></a>
  </li>
</ul>
  {% endfor %}
</section>
