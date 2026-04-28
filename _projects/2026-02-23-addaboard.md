---
title: "AddaBoard"
excerpt: "AI spatial planner."
header:
  overlay_image: /assets/images/projects/addaboard.png
  overlay_filter: 0.5
  teaser: /assets/images/projects/addaboard.png
  actions:
    - label: "Launch Web App"
      url: "https://addaboard.shahadat.us/"
sidebar:
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
  - Flutter
  - Mobile
  - Productivity
---

**AddaBoard** is an AI-powered spatial link board designed to turn your "Saved" items into actionable plans. Whether it's a recipe from Instagram, a travel spot from TikTok, or an event from a website, AddaBoard extracts the steps, ingredients, and locations automatically.

{: .notice--primary}
**What makes it different?** Unlike traditional bookmarking apps, AddaBoard focuses on *action*. It doesn't just save a link; it builds a plan.

## Key Technical Features

- **AI Extraction (V3)**: Automatically identifies Recipes, Locations, Events, and Shop items from URLs.
- **Actionable Plans**: Converts links into step-by-step checklists.
- **Immersive Reel View**: A high-speed way to browse your saved links with a glassmorphic UI.
- **Smart Categorization**: Beautifully organized cards using vibrant, AI-determined color palettes.
- **Planner Integration**: One-tap calendar additions and map routing.

## Screenshots

{% include gallery %}

## Tech Stack

- **Framework**: Flutter (Riverpod for state management)
- **Backend**: Cloudflare Workers
- **Database**: SQLite (Local Persistence)
