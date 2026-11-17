---
title: "InstaBoard"
excerpt: "AI link organizer."
header:
  overlay_image: /assets/images/projects/instaboard-header.webp
  overlay_filter: 0.75
  teaser: /assets/images/projects/instaboard-icon.webp
  actions:
    - label: "App Store"
      url: "https://apps.apple.com/us/app/instaboard-link-saver/id6760332364"
    - label: "Google Play"
      url: "https://play.google.com/store/apps/details?id=io.github.zmsp.instaboard"
    - label: "Web App"
      url: "https://save.shahadat.us"
sidebar:
  - title: "App Info"
    image: /assets/images/projects/instaboard-icon.webp
    image_alt: "InstaBoard Logo"
    text: "**Category**: Productivity / AI  \n**Platform**: iOS, Android & Web"
  - title: "Links"
    text: |
      [Web App](https://save.shahadat.us){: .btn .btn--primary .btn--block}

      [Promo Page](https://save.shahadat.us/promo){: .btn .btn--info .btn--block}
  - title: "Download"
    text: |
      [![App Store](/assets/images/app-store-badge.svg)](https://apps.apple.com/us/app/instaboard-link-saver/id6760332364)

      [![Google Play](/assets/images/google-play-badge.svg)](https://play.google.com/store/apps/details?id=io.github.zmsp.instaboard)
feature_row:
  - image_path: /assets/images/projects/instaboard-screen-1.webp
    alt: "Instant AI Extraction"
    title: "Instant AI Extraction"
    excerpt: "Automatically identifies recipes, locations, events, and shop items from shared Instagram URLs."
  - image_path: /assets/images/projects/instaboard-screen-2.webp
    alt: "Smart Categorization"
    title: "Smart Categorization"
    excerpt: "Groups saves into vivid categories tailored to the content with one-tap calendar and map integration."
gallery:
  - url: /assets/images/projects/instaboard-screen-1.webp
    image_path: /assets/images/projects/instaboard-screen-1.webp
    alt: "InstaBoard Screen 1"
  - url: /assets/images/projects/instaboard-screen-2.webp
    image_path: /assets/images/projects/instaboard-screen-2.webp
    alt: "InstaBoard Screen 2"
  - url: /assets/images/projects/instaboard-screen-3.webp
    image_path: /assets/images/projects/instaboard-screen-3.webp
    alt: "InstaBoard Screen 3"
categories:
  - software
tags:
  - AI
  - Mobile
  - Web
  - Productivity
---

**InstaBoard** is an AI-powered companion for organizing Instagram and web links. Tired of losing great tips in your "Saved" folder? Send them to InstaBoard and let our intelligent worker do the rest.

{: .notice--info}
**The Story:** We've all been there—saving a recipe, a travel location, or an event on Instagram, only for it to get lost in a sea of bookmarked posts. InstaBoard was created to turn your "Saved" list into an actionable to-do list by extracting the core utility of every link you share.

{% include figure image_path="/assets/images/projects/instaboard-header.webp" alt="InstaBoard Banner" popup=true %}

## Key Technical Features

{% include feature_row %}

* **Actionable Intelligence**: One-tap integration to add event dates to your calendar or get directions in Google Maps.
* **Privacy First**: Links are processed ephemerally with real-time metadata extraction.

## Screenshots

{% include gallery %}

## Tech Stack Deep Dive

* **Framework**: Flutter (Multi-platform)
* **State Management**: Riverpod
* **Backend**: Cloudflare Workers
* **Database**: SQLite (Local Persistence)

{% include app-cta-box.html %}
