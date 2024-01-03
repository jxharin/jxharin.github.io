# category-archive.md
---
title: "markdown"
layout: archive
permalink: /about/
author_profile: true
---

{% assign posts = site.categories.About %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}