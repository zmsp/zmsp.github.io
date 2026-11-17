---
title: "Book Shelved"
excerpt: "Personal library companion for streaming audiobooks and reading digital EPUB books."
header:
  overlay_image: /assets/images/projects/bookshelved-screen-1.webp
  overlay_filter: 0.5
  teaser: /assets/images/projects/bookshelved-icon.webp
sidebar:
  - title: "App Info"
    image: /assets/images/projects/bookshelved-icon.webp
    image_alt: "Book Shelved Logo"
    text: "**Category**: Books  \n**Privacy**: 100% Private  \n**Platform**: iOS & Android"
  - title: "Links"
    text: "[Apps Page](https://apps.shahadat.us/apps/bookshelved/){: .btn .btn--info .btn--large}"
  - title: "Download"
    text: "[![App Store](/assets/images/app-store-icon.svg)](https://apps.apple.com/us/app/shelved-audiobooks-books/id6798978127){: style='width: 40px; display: inline-block; margin-right: 10px;'} [![Google Play](/assets/images/google-play-icon.svg)](https://play.google.com/store/apps/details?id=io.github.zmsp.books){: style='width: 33px; display: inline-block;'}"
gallery:
  - url: /assets/images/projects/bookshelved-screen-1.webp
    image_path: /assets/images/projects/bookshelved-screen-1.webp
    alt: "Shelved Library Overview"
  - url: /assets/images/projects/bookshelved-screen-2.webp
    image_path: /assets/images/projects/bookshelved-screen-2.webp
    alt: "Audiobook Player Interface"
toc: true
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

## Key Features

* **Seamless Audiobook Player**: Background audio streaming, variable playback speed controls, sleep timer, and fine-grained position tracking.
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
