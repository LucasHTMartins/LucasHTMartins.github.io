---
title: "Projects"
layout: single
author_profile: true
no_posts: true
---


Here you can find detailed summaries of my programming and computer science projects.

<ul>
  {% for project in site.projects %}
    <li><a href="{{ project.url }}">{{ project.title }}</a></li>
  {% endfor %}
</ul>
