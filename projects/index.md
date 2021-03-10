---
layout: page
title: AI 101 Series for Dummies
description: Series of blogposts to understand complex AI/ML topics in a clear and concise manner.
permalink: /projects/
---

I love to build software, experiment with data, and implement machine
learning systems. Check-out some of my works!

<ul>
  {% for post in site.categories.projects %}
    <li>
        <span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
        <meta name="description" content="{{ post.summary | escape }}">
        <meta name="keywords" content="{{ post.tags | join: ', ' | escape }}"/>
    </li>
  {% endfor %}
</ul>