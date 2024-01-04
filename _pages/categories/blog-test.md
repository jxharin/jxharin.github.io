---
title: "blog"
layout: archive
permalink: categories/blog
---
{% assign posts = site.categories.blog %}
{% for post in posts %} {% include archive-single2.html type=page.entries_layout %} {% endfor %}