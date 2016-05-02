---
layout: page
title: All posts
permalink: /all_posts/
---

Esta sección contiene una lista con todos los posts escritos hasta el momento:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
