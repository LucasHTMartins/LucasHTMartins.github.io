---
title: "Blog"
layout: home
author_profile: true
no_posts: true
---

Here you’ll find personal news and updates related to my recent adventures.

<ul>
  {% for post in site.blog %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
