---
title: "AppRankly — Open-Source App Store Analytics & ASO Studio"
excerpt: "Stop constantly switching between App Store Connect and Google Play Console. AppRankly brings your iOS and Android performance metrics together into a single, self-hosted dashboard."
header:
  overlay_image: /assets/images/projects/apprankly-screen-1.webp
  overlay_filter: 0.75
  teaser: /assets/images/projects/apprankly-icon.webp
  actions:
    - label: "GitHub"
      url: "https://github.com/zmsp/AppRankly"
    - label: "Live Demo"
      url: "https://zmsp.github.io/AppRankly/#demo"
sidebar:
  - title: "App Info"
    image: /assets/images/projects/apprankly-icon.webp
    image_alt: "AppRankly Logo"
    text: "**Category**: Developer Tools  \n**License**: MIT Open Source  \n**Platform**: Self-Hosted Web, Docker & Unraid"
  - title: "Links"
    text: |
      [GitHub Repository](https://github.com/zmsp/AppRankly){: .btn .btn--primary .btn--block}

      [Live Interactive Demo](https://zmsp.github.io/AppRankly/#demo){: .btn .btn--success .btn--block}

      [Apps Page](https://apps.shahadat.us/apps/apprankly/){: .btn .btn--info .btn--block}

      [Unraid App Listing](https://ca.unraid.net/apps/apprankly-1bdjnw60t14ouy){: .btn .btn--warning .btn--block}

      [Docker Container](https://github.com/zmsp/AppRankly/pkgs/container/apprankly){: .btn .btn--danger .btn--block}
feature_row:
  - image_path: /assets/images/projects/apprankly-screen-1.webp
    alt: "Unified Analytics Dashboard Overview"
    title: "Unified App Store Metrics"
    excerpt: "Pull data directly from Google Cloud Storage (Google Play) and the App Store Connect API into a single clean performance overview."
  - image_path: /assets/images/projects/apprankly-screen-2.webp
    alt: "AI-Powered ASO Keyword & Metadata Studio"
    title: "AI-Powered ASO Studio"
    excerpt: "Discover keyword ideas using live store autocomplete data, run listing health checks, and draft metadata with OpenAI, Anthropic, or Gemini."
gallery:
  - url: /assets/images/projects/apprankly-screen-1.webp
    image_path: /assets/images/projects/apprankly-screen-1.webp
    alt: "Unified Analytics Dashboard Overview"
  - url: /assets/images/projects/apprankly-screen-2.webp
    image_path: /assets/images/projects/apprankly-screen-2.webp
    alt: "AI-Powered ASO Keyword & Metadata Studio"
categories:
  - software
tags:
  - Analytics
  - Mobile
  - ASO
  - Self-Hosted
  - Docker
  - Unraid
  - Open Source
  - Node.js
---

> **Live Demo**: Try the interactive web dashboard instantly: **[AppRankly Live Demo](https://zmsp.github.io/AppRankly/#demo)** *(Running in simulated demo mode with sample data)*  
> **Links**: [GitHub Repository](https://github.com/zmsp/AppRankly) | [Apps Directory](https://apps.shahadat.us/apps/apprankly/) | [Unraid Store](https://ca.unraid.net/apps/apprankly-1bdjnw60t14ouy) | [Docker Image](https://github.com/zmsp/AppRankly/pkgs/container/apprankly)

## AppRankly

Stop constantly switching between App Store Connect and Google Play Console. **AppRankly** brings your iOS and Android performance metrics together into a single, self-hosted dashboard. Track installs, audit listing health, and uncover high-ranking keywords—all while keeping your API keys and analytics 100% private on your own server.

## Key Features

{% include feature_row %}

* **Unified App Store Metrics**: Track installs, uninstalls, active devices, and country-by-country breakdowns for both iOS and Android in one view.
* **AI-Powered ASO Studio**: Discover keyword ideas using live store autocomplete data, run instant listing audits, and generate AI-optimized app metadata with OpenAI, Anthropic, or Gemini.
* **100% Self-Hosted & Private**: Your credentials and metrics stay strictly on your server. No third-party trackers, no telemetry, no data collection.
* **Docker & Unraid Container Ready**: Spin up in under a minute using Docker Compose, GHCR images, or [Unraid Community Applications](https://ca.unraid.net/apps/apprankly-1bdjnw60t14ouy).
* **CLI & Automation**: Run background syncs, export raw reports, or trigger scheduled daily updates using standard cron jobs.

## Screenshots

{% include gallery %}

## Tech Stack

* **Frontend**: HTML5, Vanilla CSS3, JavaScript (Lightweight Glassmorphic SPA)
* **Backend**: Node.js & Express REST API
* **AI Integrations**: OpenAI, Anthropic (Claude), and Google Gemini
* **Deployment**: Docker, Docker Compose, GHCR, Unraid CA

{% include app-cta-box.html
   web_url="https://zmsp.github.io/AppRankly/#demo"
   web_label="Launch Live Demo"
   github="https://github.com/zmsp/AppRankly"
%}
