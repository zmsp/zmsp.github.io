---
title: "Salah Time — Qibla, Adhan & Focus Shield"
excerpt: "Accurate prayer times, Kaaba Qibla finder, and distraction-free prayer locks powered by Apple Screen Time."
header:
  overlay_image: /assets/images/projects/salahtime-screen-1.webp
  overlay_filter: 0.5
  teaser: /assets/images/projects/salahtime-icon.webp
sidebar:
  - title: "App Info"
    image: /assets/images/projects/salahtime-icon.webp
    image_alt: "Salah Time Logo"
    text: "**Category**: Utilities  \n**Privacy**: 100% On-Device / No Tracking  \n**Platform**: iOS (iPhone & iPad)"
  - title: "Links"
    text: "[GitHub Repository](https://github.com/zmsp/salahtime){: .btn .btn--primary .btn--large}\n\n[Apps Page](https://apps.shahadat.us/apps/salahtime/){: .btn .btn--info .btn--large}"
  - title: "Download"
    text: "[![App Store](/assets/images/app-store-icon.svg)](https://apps.apple.com/us/app/salah-time/id6810905983){: style='width: 40px; display: inline-block;'}"
gallery:
  - url: /assets/images/projects/salahtime-screen-1.webp
    image_path: /assets/images/projects/salahtime-screen-1.webp
    alt: "Prayer Timetable Overview"
  - url: /assets/images/projects/salahtime-screen-2.webp
    image_path: /assets/images/projects/salahtime-screen-2.webp
    alt: "Screen Time Prayer Shield"
toc: true
categories:
  - software
tags:
  - Mobile
  - iOS
  - Swift
  - SwiftUI
  - Screen Time
  - Privacy
  - Utilities
---

A lot of Islamic apps are loaded with ads or constantly asking for your location in the background. And even if you get past that, the phone is still buzzing with notifications during prayer.

**Salah Time** is a no-frills prayer companion for iOS. It calculates times on-device, points you toward the Qibla, and can lock distracting apps during prayer windows using Apple's Screen Time API. No ads, no tracking, no cloud.

## Key Features

* **Astronomical Prayer Calculations**: Calculates Fajr, Sunrise, Dhuhr, Asr, Maghrib, and Isha directly on-device using trusted global calculation conventions (MWL, ISNA, Umm al-Qura Makkah, Egyptian General Authority, University of Islamic Sciences Karachi).
* **Screen Time Prayer Shield**: Temporarily shields social media and distracting apps during prayer windows using Apple's native Screen Time framework (`FamilyControls`, `ManagedSettings`, and `DeviceActivity`) for undistracted worship.
* **Calibrated Kaaba Qibla Locator**: Real-time magnetometer compass pointing directly toward the Kaaba in Mecca, complete with subtle haptic vibration cues upon exact alignment.
* **Tactile Digital Tasbih**: Built-in Dhikr counter featuring smooth counting animations, milestone lap vibration feedback, and essential remembrance presets.
* **Authentic Dua Collection**: Access categorized daily supplications featuring verified Arabic text, clear phonetic transliteration, and English translations.
* **100% Private & Ad-Free**: Zero tracking, zero telemetry, no third-party SDKs, and zero cloud backends. Your location and usage data never leave your device.

## Screenshots

{% include gallery %}

## Tech Stack

* **Language**: Swift
* **UI Framework**: SwiftUI & Combine
* **Apple Frameworks**: Screen Time (`FamilyControls`, `ManagedSettings`, `DeviceActivity`), CoreLocation, CoreMotion
* **Architecture**: Clean MVVM with local persistent storage
* **Platform**: iOS & iPadOS
