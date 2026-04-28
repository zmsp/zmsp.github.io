---
title: "InstaBoard"
excerpt: "AI link organizer."
header:
  overlay_image: /assets/images/projects/instaboard.jpg
  overlay_filter: 0.5
  teaser: /assets/images/projects/instaboard.jpg
  actions:
    - label: "Launch Web App"
      url: "https://save.shahadat.us"
sidebar:
  - title: "Links"
    text: "[Web App](https://save.shahadat.us)  \n[Promo](https://save.shahadat.us/promo)"
  - title: "Download"
    text: "[![App Store](/assets/images/app-store-icon.svg)](https://apps.apple.com/us/app/instaboard-link-saver/id6760332364){: style='width: 40px; display: inline-block; margin-right: 10px;'} [![Google Play](/assets/images/google-play-icon.svg)](https://play.google.com/store/apps/details?id=io.github.zmsp.instaboard){: style='width: 33px; display: inline-block;'}"
  - title: "Tech Stack"
    image: /assets/images/projects/instaboard-logo.jpg
    image_alt: "InstaBoard Logo"
    text: "**Framework**: Flutter  \n**Backend**: Cloudflare Workers  \n**Database**: SQLite"
gallery:
  - url: /assets/images/projects/instaboard-screenshot1.jpg
    image_path: /assets/images/projects/instaboard-screenshot1.jpg
    alt: "InstaBoard Screenshot 1"
  - url: /assets/images/projects/instaboard-screenshot2.jpg
    image_path: /assets/images/projects/instaboard-screenshot2.jpg
    alt: "InstaBoard Screenshot 2"
toc: true
categories:
  - software
tags:
  - AI
  - Flutter
  - Mobile
  - Productivity
---

**InstaBoard** is an AI-powered companion for organizing Instagram and web links. Tired of losing great tips in your "Saved" folder? Send them to InstaBoard and let our intelligent worker do the rest.

{: .notice--info}
**The Story:** We've all been there—saving a recipe, a travel location, or an event on Instagram, only for it to get lost in a sea of bookmarked posts. InstaBoard was created to turn your "Saved" list into an actionable to-do list by extracting the core utility of every link you share.

## Key Technical Features

- **Instant AI Extraction**: Automatically identifies Recipes, Locations, Events, and Shop items from URLs.
- **Smart Categorization**: Groups saves into vivid, intelligently-colored categories tailored to the content.
- **Actionable Intelligence**: One-tap integration to add event dates to your calendar or get directions in Google Maps.
- **Privacy First**: Links are processed ephemerally with real-time metadata extraction.

## Screenshots

{% include gallery %}

## Tech Stack Deep Dive

- **Framework**: Flutter (Multi-platform)
- **State Management**: Riverpod
- **Backend**: Cloudflare Workers
- **Database**: SQLite (Local Persistence)
