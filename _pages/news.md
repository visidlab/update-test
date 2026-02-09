---
title: "News"
permalink: /news/
layout: posts
entries_layout: list
---

{% assign posts = site.news | default: site.posts | sort: "date" | reverse %}
{% for post in posts %}
  {% include archive-single.html type="news" %}
{% endfor %}