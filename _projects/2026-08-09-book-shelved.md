---
title: "Book Shelved"
excerpt: "Personal library companion for streaming audiobooks and reading digital EPUB books."
header:
  overlay_image: /assets/images/projects/bookshelved-header.webp
  overlay_filter: 0.75
  teaser: /assets/images/projects/bookshelved-icon.webp
  actions:
    - label: "App Store"
      url: "https://apps.apple.com/us/app/shelved-audiobookshelf-reader/id6798978127"
    - label: "Google Play"
      url: "https://play.google.com/store/apps/details?id=io.github.zmsp.books"
sidebar:
  - title: "App Info"
    image: /assets/images/projects/bookshelved-icon.webp
    image_alt: "Book Shelved Logo"
    text: "**Category**: Books  \n**Privacy**: 100% Private  \n**Platform**: iOS & Android"
  - title: "Links"
    text: "[Apps Page](https://apps.shahadat.us/apps/bookshelved/){: .btn .btn--info .btn--block}"
  - title: "Download"
    text: |
      [![App Store](/assets/images/app-store-badge.svg)](https://apps.apple.com/us/app/shelved-audiobookshelf-reader/id6798978127)

      [![Google Play](/assets/images/google-play-badge.svg)](https://play.google.com/store/apps/details?id=io.github.zmsp.books)
feature_row:
  - image_path: /assets/images/projects/bookshelved-screen-1.webp
    alt: "Shelved Library Overview"
    title: "Audiobook & eBook Library"
    excerpt: "Connect directly to your self-hosted server like Audiobookshelf. Stream or download books for offline reading and listening."
  - image_path: /assets/images/projects/bookshelved-screen-2.webp
    alt: "Audiobook Player Interface"
    title: "Seamless Audio Player"
    excerpt: "Background audio streaming, variable playback speeds, sleep timer, and fine-grained position tracking synced across devices."
gallery:
  - url: /assets/images/projects/bookshelved-screen-1.webp
    image_path: /assets/images/projects/bookshelved-screen-1.webp
    alt: "Shelved Library Overview"
  - url: /assets/images/projects/bookshelved-screen-2.webp
    image_path: /assets/images/projects/bookshelved-screen-2.webp
    alt: "Audiobook Player Interface"
categories:
  - software
tags:
  - Mobile
  - Books
  - Audiobooks
  - EPUB
  - Flutter
  - Material 3
---

I use Audiobookshelf to self-host my audiobook and ebook library, and there wasn't a great mobile client for it. Most apps either only do audiobooks or only do EPUBs, and the ones that do both are pretty clunky.

**Book Shelved** (Shelved) is what I ended up building. It connects to your personal media server, handles both audiobooks and EPUBs, and tries to stay out of your way so you can just read or listen.

{% include figure image_path="/assets/images/projects/bookshelved-header.webp" alt="Book Shelved Banner" popup=true %}

## Key Features

{% include feature_row %}

* **Integrated EPUB Reader**: Full-featured digital reader with customizable typography, theme modes (Light, Dark, OLED Black), and chapter-by-chapter navigation.
* **Offline Mode & Downloads**: Download complete audiobooks and eBooks directly to your device for offline listening and reading during flights or commutes.
* **Library & Server Syncing**: Connect directly to your personal home media server (such as Audiobookshelf) to sync listening and reading progress across multiple devices.
* **Modern Material 3 Interface**: Smooth animations, dynamic color themes, and responsive design tailored for phones and tablets.

## Screenshots

{% include gallery %}

## Tech Stack

* **Framework**: Flutter & Dart
* **Design System**: Material 3 Design
* **Audio Engine**: Just Audio with background audio session management
* **Protocols**: Audiobookshelf REST API & Local Storage Cache
* **Platforms**: iOS (iPhone & iPad) & Android

{% include app-cta-box.html %}
