---
title: "Projects"
layout: single
author_profile: true
no_posts: true
---

Follow the links below for a summary of my programming and computer science projects.

<ul>
  {% assign sorted_projects = site.projects | sort: 'name' | reverse %}
  {% for project in sorted_projects %}
    <li><a href="{{ project.url }}">{{ project.title }}</a></li>
  {% endfor %}
</ul>

