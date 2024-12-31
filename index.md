---
layout: default
title: Home
---

# Welcome to My Website

This is the home page content.

## Blog Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>{{ post.date | date: "%-d %B %Y" }}</small>
    </li>
  {% endfor %}
</ul>