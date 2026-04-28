---
title: "Projects by Tag"
permalink: /projects/tags/
layout: archive
author_profile: true
entries_layout: grid
header:
  overlay_image: /assets/images/unslpash/unsplash-image-1.jpg
  overlay_filter: 0.6
---

{% assign all_tags = "" %}
{% for post in site.projects %}
{% for tag in post.tags %}
{% capture all_tags %}{{ all_tags }}{{ tag }},{% endcapture %}
{% endfor %}
{% endfor %}
{% assign tags = all_tags | split: "," | uniq | sort %}

<ul class="taxonomy__index">
{% for tag in tags %}{% if tag != "" %}
<li>
<a href="#{{ tag | slugify }}">
<strong>{{ tag }}</strong> <span class="taxonomy__count">{% assign count = 0 %}{% for post in site.projects %}{% if post.tags contains tag %}{% assign count = count | plus: 1 %}{% endif %}{% endfor %}{{ count }}</span>
</a>
</li>
{% endif %}{% endfor %}
</ul>

{% for tag in tags %}{% if tag != "" %}
<section id="{{ tag | slugify }}" class="taxonomy__section">
<h2 class="archive__subtitle">{{ tag }}</h2>
<div class="entries-grid">
{% for post in site.projects %}{% if post.tags contains tag %}
{% include archive-single.html type="grid" %}
{% endif %}{% endfor %}
</div>
<a href="#page-title" class="back-to-top">{{ site.data.ui-text[site.locale].back_to_top | default: 'Back to Top' }} &uarr;</a>
</section>
{% endif %}{% endfor %}

