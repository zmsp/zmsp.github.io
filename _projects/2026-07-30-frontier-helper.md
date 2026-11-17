---
title: "Frontier Helper"
excerpt: "The ultimate flight, route, and booking window companion for Frontier GoWild! pass holders."
header:
  overlay_image: /assets/images/projects/frontierhelper-header.webp
  overlay_filter: 0.5
  teaser: /assets/images/projects/frontierhelper-icon.webp
sidebar:
  - title: "App Info"
    image: /assets/images/projects/frontierhelper-icon.webp
    image_alt: "Frontier Helper Logo"
    text: "**Category**: Travel  \n**Privacy**: 100% On-Device  \n**Platform**: iOS & Android"
  - title: "Links"
    text: "[Apps Page](https://apps.shahadat.us/apps/frontierhelper/){: .btn .btn--info .btn--large}"
  - title: "Download"
    text: "[![App Store](/assets/images/app-store-icon.svg)](https://apps.apple.com/us/app/frontier-helper/id6796272726){: style='width: 40px; display: inline-block; margin-right: 10px;'} [![Google Play](/assets/images/google-play-icon.svg)](https://play.google.com/store/apps/details?id=io.github.zmsp.frontierhelper){: style='width: 33px; display: inline-block;'}"
gallery:
  - url: /assets/images/projects/frontierhelper-screen-1.webp
    image_path: /assets/images/projects/frontierhelper-screen-1.webp
    alt: "GoWild Route & Flight Finder"
  - url: /assets/images/projects/frontierhelper-screen-2.webp
    image_path: /assets/images/projects/frontierhelper-screen-2.webp
    alt: "Booking Window & Blackout Calendar"
toc: true
categories:
  - software
tags:
  - Mobile
  - Travel
  - Aviation
  - Flights
  - Flutter
  - Offline-First
---

The GoWild! pass rules are honestly confusing. Domestic flights only open up 1 day before departure, international ones open 10 days out, and there are blackout dates scattered throughout the year. I kept second-guessing myself every time I wanted to book.

So I built **Frontier Helper** to keep track of all that for me. It shows available routes, the booking window calendar, and lets me pull up my boarding pass QR without digging through emails.

![Frontier Helper Banner](/assets/images/projects/frontierhelper-header.webp)

## Key Features

* **GoWild! Route & Flight Finder**: Discover eligible Frontier routes across North America and Latin America, and search available flights from your home base airport.
* **Booking Window & Blackout Calendar**: Track domestic (0–2 days) and international (0–11 days) booking windows alongside official GoWild blackout dates on an interactive calendar.
* **Traveler Pass & Boarding Pass Wallet**: Save Frontier IDs, TSA PreCheck numbers, and scan or crop boarding pass QR codes securely right on your device.
* **Live Flight Status Lookup**: Check real-time ADS-B telemetry, squawk codes, flight status, and route maps for your saved flights.
* **100% On-Device & Private**: All profile details, saved flight data, and boarding pass scans stay stored locally on your device.

## Screenshots

{% include gallery %}

## Tech Stack

* **Frontend**: Flutter & Riverpod
* **Data & Storage**: SQLite & On-Device Caching
* **Flight Data**: ADS-B Telemetry & Route Graph Engine
* **Platforms**: iOS (iPhone & iPad) & Android
