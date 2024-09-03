---
title: "Blog"
layout: home
author_profile: true

---

Welcome to my blog! Here you’ll find personal news and updates related to my recent adventures.



<ul>
  {% for post in site.blog %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
