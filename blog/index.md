---
title: "Blog"
layout: single
---

Welcome to my blog! Here you’ll find personal news and updates related to my recent adventures.



<ul>
  {% for post in site.posts %}
    {% if post.path contains '/blog/' %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
      </li>
    {% endif %}
  {% endfor %}
</ul>
