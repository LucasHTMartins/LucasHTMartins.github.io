---
title: "Projects"
layout: single
---


Here you can find detailed summaries of my programming and computer science projects.

<ul>
  {% for post in site.posts %}
    {% if post.path contains '/projects/' %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
      </li>
    {% endif %}
  {% endfor %}
</ul>
