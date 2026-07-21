---
title: "CardTrack"
excerpt: "Track credit card rewards, statement credits, bonus points, and merchant offers in one private dashboard."
header:
  overlay_image: /assets/images/projects/cardtrack-screen-1.webp
  overlay_filter: 0.5
  teaser: /assets/images/projects/cardtrack-icon.webp
sidebar:
  - title: "App Info"
    image: /assets/images/projects/cardtrack-icon.webp
    image_alt: "CardTrack Logo"
    text: "**Category**: Finance  \n**Privacy**: 100% Local / Offline-First  \n**Platform**: iOS & Android"
  - title: "Download"
    text: "[![App Store](/assets/images/app-store-icon.svg)](https://apps.apple.com/us/app/cardtrack/id6789731069){: style='width: 40px; display: inline-block; margin-right: 10px;'} [![Google Play](/assets/images/google-play-icon.svg)](https://play.google.com/store/apps/details?id=io.github.zmsp.cardtrack){: style='width: 33px; display: inline-block;'}"
gallery:
  - url: /assets/images/projects/cardtrack-screen-1.webp
    image_path: /assets/images/projects/cardtrack-screen-1.webp
    alt: "CardTrack Overview"
  - url: /assets/images/projects/cardtrack-screen-2.webp
    image_path: /assets/images/projects/cardtrack-screen-2.webp
    alt: "CardTrack Expiration Reminders"
  - url: /assets/images/projects/cardtrack-screen-3.webp
    image_path: /assets/images/projects/cardtrack-screen-3.webp
    alt: "CardTrack Best Card Recommendation"
toc: true
categories:
  - software
tags:
  - Mobile
  - Finance
  - Rewards
  - Flutter
  - Privacy
  - Offline-First
---

Managing multiple credit cards and trying to remember every monthly dining credit, annual travel perk, or quarterly bonus category can quickly become overwhelming. Premium financial apps often require linking sensitive bank credentials, while spreadsheets are tedious to maintain.

To solve this, I built **CardTrack** — a private, offline-first dashboard designed to help you maximize every credit card benefit you already own without sacrificing privacy or sharing bank logins.

## Key Features

* **100% On-Device & Private**: CardTrack requires no account creation, no bank logins, and no cloud syncing. All your card holdings and custom offer tracking stay locked safely on your device.
* **Smart Benefit & Credit Tracking**: Keep tabs on recurring statement credits (travel, dining, streaming, Uber, etc.), annual free night certificates, and merchant offers across all your cards.
* **Automatic Expiration Reminders**: Set up custom notifications so statement credits, annual perks, and limited-time bonus offers never slip away unredeemed.
* **Best Card for Purchase Lookup**: Quick decision helper to instantly determine which of your active cards yields the highest cashback percentage or points multiplier for specific purchase categories.
* **Comprehensive Issuer Catalog**: Built-in templates for 50+ popular credit cards across 15+ major issuers, allowing instant setup.

## Screenshots

{% include gallery %}

## Tech Stack

* **Framework**: Flutter & Riverpod (for responsive UI and robust local state management)
* **Database**: Isar (high-performance embedded local database for offline persistence)
* **Platforms**: iOS (iPhone & iPad) & Android
