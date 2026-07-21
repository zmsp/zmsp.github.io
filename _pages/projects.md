---
title: "Projects"
layout: archive
permalink: /projects/
collection: projects
entries_layout: grid
classes: wide
author_profile: true
header:
  overlay_image: /assets/images/unslpash/unsplash-image-1.jpg
  overlay_filter: 0.5
  actions:
    - label: "Browse by Tag"
      url: "/projects/tags/"
excerpt: "A collection of my latest work, from open-source tools to hardware projects."
sort_by: date
sort_order: reverse
---

Welcome to my portfolio. Here you'll find a selection of my software and hardware projects, ranging from AI applications to system-level tools.

<div class="grid__wrapper">
  {% assign entries = site.projects | sort: 'date' | reverse %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
