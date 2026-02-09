---
title: "News"
permalink: /news/
layout: archive
entries_layout: list
---

{% assign posts = site.news | default: site.posts | sort: "date" | reverse %}
<div class="entries-{{ page.entries_layout | default: 'list' }}">
  {% for post in posts %}
    {% include archive-single.html type=page.entries_layout %}
  {% endfor %}
</div>