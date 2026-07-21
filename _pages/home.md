---
layout: splash
permalink: /
hidden: true
classes: wide
header:
  overlay_image: /assets/images/unslpash/unsplash-image-3.jpg
  overlay_filter: 0.5
  title: "TIL | ZOBAIR"
  excerpt: "A journey through code and creativity. Hi there! I'm Zobair. I share my evolution through engineering experiments and public learning."
  actions:
    - label: "Explore Projects"
      url: "/projects/"
    - label: "Read Notes"
      url: "/blogs/"
    - label: "GitHub"
      url: "https://github.com/zmsp"
feature_row:
  - image_path: /assets/images/projects/cardtrack-icon.webp
    alt: "CardTrack"
    title: "CardTrack"
    excerpt: "Track credit card rewards, statement credits, bonus points, and merchant offers in one private dashboard."
    url: "/projects/2026-07-21-cardtrack/"
    btn_class: "btn--primary"
    btn_label: "Learn More"
  - image_path: /assets/images/projects/triptale-icon.png
    alt: "TripTale Map"
    title: "TripTale Map"
    excerpt: "Privacy-first, offline-first travel journal and memory reconstruction app."
    url: "/projects/2026-07-17-triptale/"
    btn_class: "btn--primary"
    btn_label: "Learn More"
  - image_path: /assets/images/projects/triviathon-icon.webp
    alt: "Triviathon"
    title: "Triviathon"
    excerpt: "Fast-paced trivia and quiz game."
    url: "/projects/2026-05-02-triviathon/"
    btn_class: "btn--primary"
    btn_label: "Learn More"
---

<div class="archive">
  <h2 class="archive__subtitle">Projects</h2>
  <p>Explore featured software applications, from AI experiments to handy developer tools.</p>
</div>

{% include feature_row %}

<hr style="margin: 3em 0; border: 0; border-top: 1px solid rgba(0, 0, 0, 0.12);" />

<div class="archive">
  <h2 class="archive__subtitle">Learning Notes</h2>
  <p>Here are my recent deep dives into the world of tech.</p>
  <div class="entries-list">
    {% assign recent_posts = site.posts | sort: 'date' | reverse %}
    {% for post in recent_posts limit: 5 %}
      {% include archive-single.html type="list" %}
    {% endfor %}
  </div>
  <p style="margin-top: 1.5em;"><a href="{{ '/blogs/' | relative_url }}" class="btn btn--primary">Browse All Learning Notes</a></p>
</div>
