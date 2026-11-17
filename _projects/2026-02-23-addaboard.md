---
title: "AddaBoard — Trip & Event Spatial Planner"
excerpt: "Visual spatial planner for turning saved ideas into plans. Extract recipes, itineraries, and events into an actionable board."
header:
  overlay_image: /assets/images/projects/addaboard-screenshot.webp
  overlay_filter: 0.75
  teaser: /assets/images/projects/addaboard-icon.webp
  actions:
    - label: "App Store"
      url: "https://apps.apple.com/us/app/addaboard-trip-event-plan/id6760598074"
    - label: "Google Play"
      url: "https://play.google.com/store/apps/details?id=io.github.zmsp.addaboard"
    - label: "Web App"
      url: "https://addaboard.shahadat.us/"
sidebar:
  - title: "App Info"
    image: /assets/images/projects/addaboard-icon.webp
    image_alt: "AddaBoard Logo"
    text: "**Category**: Productivity / AI  \n**Platform**: iOS, Android & Web"
  - title: "Links"
    text: |
      [Web App](https://addaboard.shahadat.us/){: .btn .btn--primary .btn--block}

      [Apps Page](https://apps.shahadat.us/apps/addaboard/){: .btn .btn--info .btn--block}

      [Promo Page](https://addaboard.shahadat.us/promo){: .btn .btn--info .btn--block}
  - title: "Download"
    text: |
      [![App Store](/assets/images/app-store-badge.svg)](https://apps.apple.com/us/app/addaboard-trip-event-plan/id6760598074)

      [![Google Play](/assets/images/google-play-badge.svg)](https://play.google.com/store/apps/details?id=io.github.zmsp.addaboard)
feature_row:
  - image_path: /assets/images/projects/adda_board-screen-1.webp
    alt: "AddaBoard Smart Extraction"
    title: "Smart Link Extraction"
    excerpt: "Pulls out recipe steps, ingredients, or locations automatically from saved social posts so you can take action."
  - image_path: /assets/images/projects/adda_board-screen-2.webp
    alt: "AddaBoard Visual Planning"
    title: "Visual Reel Planning"
    excerpt: "Immersive reel view makes browsing your saved ideas as fast and fluid as the social apps you found them on."
gallery:
  - url: /assets/images/projects/addaboard-screenshot.webp
    image_path: /assets/images/projects/addaboard-screenshot.webp
    alt: "AddaBoard Screenshot"
  - url: /assets/images/projects/adda_board-screen-1.webp
    image_path: /assets/images/projects/adda_board-screen-1.webp
    alt: "AddaBoard Feature Screen 1"
  - url: /assets/images/projects/adda_board-screen-2.webp
    image_path: /assets/images/projects/adda_board-screen-2.webp
    alt: "AddaBoard Feature Screen 2"
categories:
  - software
tags:
  - AI
  - Mobile
  - Web
  - Productivity
---

**AddaBoard** started as a personal solution to a common problem: I was saving hundreds of links to recipes, travel spots, and events on Instagram and TikTok, but I never actually looked at them again. I wanted a way to turn those "saved" items into real, actionable plans.

What began as a side project (originally named *InstaBoard*) has grown into my most significant production app.

## Key Features

{% include feature_row %}

* **Action-Oriented**: Everything is designed to be a checklist. One tap to add a recipe ingredient to your grocery list or a travel spot to your maps.
* **Multi-Platform**: Available on iOS, Android, and Web with instant synchronization.

## Screenshots

{% include gallery %}

## Tech Stack

* **Framework**: Flutter (Riverpod for state management)
* **Backend**: Cloudflare Workers
* **Database**: SQLite (Local Persistence)

{% include app-cta-box.html %}
