---
title: "Projects"
layout: single
author_profile: true
no_posts: true
---

Follow the links below for a summary of my programming and computer science projects.

<ul>
  {% for project in site.projects %}
    <li><a href="{{ project.url }}">{{ project.title }}</a></li>
  {% endfor %}
</ul>
