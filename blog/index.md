---
title: "Blog"
layout: home
author_profile: true
no_posts: true
---

Here you’ll find personal news, updates, and other miscellaneous posts.

<ul>
  {% assign sorted_posts = site.blog | sort: 'name' | reverse %}
  {% for post in sorted_posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
