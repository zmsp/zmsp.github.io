---
title: "AddaBoard"
excerpt: "AI spatial planner."
header:
  overlay_image: /assets/images/projects/addaboard.png
  overlay_filter: 0.5
  teaser: /assets/images/projects/placeholder_small.jpeg
  actions:
    - label: "Launch Web App"
      url: "https://addaboard.shahadat.us/"
sidebar:
  - title: "Links"
    text: "[Web App](https://addaboard.shahadat.us/)  \n[Promo](https://addaboard.shahadat.us/promo)"
  - title: "Download"
    text: "[![App Store](/assets/images/app-store-icon.svg)](https://apps.apple.com/us/app/adda-board-link-planner/id6760598074){: style='width: 40px; display: inline-block; margin-right: 10px;'} [![Google Play](/assets/images/google-play-icon.svg)](https://play.google.com/store/apps/details?id=io.github.zmsp.addaboard){: style='width: 33px; display: inline-block;'}"
  - title: "Tech Stack"
    image: /assets/images/projects/addaboard-logo.png
    image_alt: "AddaBoard Logo"
    text: "**Framework**: Flutter  \n**Backend**: Cloudflare Workers  \n**Database**: SQLite"
gallery:
  - url: /assets/images/projects/addaboard.png
    image_path: /assets/images/projects/addaboard.png
    alt: "AddaBoard Promo"
  - url: /assets/images/projects/addaboard-screenshot2.png
    image_path: /assets/images/projects/addaboard-screenshot2.png
    alt: "Screenshot 2"
  - url: /assets/images/projects/addaboard-screenshot3.png
    image_path: /assets/images/projects/addaboard-screenshot3.png
    alt: "Screenshot 3"
  - url: /assets/images/projects/addaboard-screenshot4.png
    image_path: /assets/images/projects/addaboard-screenshot4.png
    alt: "Screenshot 4"
  - url: /assets/images/projects/addaboard-screenshot5.png
    image_path: /assets/images/projects/addaboard-screenshot5.png
    alt: "Screenshot 5"
toc: true
categories:
  - software
tags:
  - AI
  - Mobile
  - Web
  - Productivity
---

**AddaBoard** started as a personal solution to a common problem: I was saving hundreds of links to recipes, travel spots, and events on Instagram and TikTok, but I never actually looked at them again. I wanted a way to turn those "saved" items into real, actionable plans.

What began as a side project (originally named *InstaBoard*) has grown into my most significant production app



### What it does
- **Smart Extraction**: It doesn't just save a link; it pulls out the steps, ingredients, or locations automatically so you can get moving.
- **Visual Planning**: I built an "Immersive Reel" view that makes browsing your saved plans feel as fast and fluid as the social apps you found them on.
- **Action-Oriented**: Everything is designed to be a checklist. One tap to add a recipe ingredient to your grocery list or a travel spot to your maps.

## Tech Stack

- **Framework**: Flutter (Riverpod for state management)
- **Backend**: Cloudflare Workers
- **Database**: SQLite (Local Persistence)
