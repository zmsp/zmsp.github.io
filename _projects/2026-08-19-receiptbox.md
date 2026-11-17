---
title: "ReceiptBox"
excerpt: "Private on-device receipt scanner, expense manager, and bill splitter."
header:
  overlay_image: /assets/images/projects/receiptbox-screen-1.webp
  overlay_filter: 0.75
  teaser: /assets/images/projects/receiptbox-icon.webp
  actions:
    - label: "App Store"
      url: "https://apps.apple.com/us/app/receiptbox/id6802949285"
    - label: "Google Play"
      url: "https://play.google.com/store/apps/details?id=io.github.zmsp.receiptbox&hl=en_US"
sidebar:
  - title: "App Info"
    image: /assets/images/projects/receiptbox-icon.webp
    image_alt: "ReceiptBox Logo"
    text: "**Category**: Finance  \n**Privacy**: 100% On-Device / Offline  \n**Platform**: iOS & Android"
  - title: "Links"
    text: "[Apps Page](https://apps.shahadat.us/apps/receiptbox/){: .btn .btn--info .btn--block}"
  - title: "Download"
    text: |
      [![App Store](/assets/images/app-store-badge.svg)](https://apps.apple.com/us/app/receiptbox/id6802949285)

      [![Google Play](/assets/images/google-play-badge.svg)](https://play.google.com/store/apps/details?id=io.github.zmsp.receiptbox&hl=en_US)
feature_row:
  - image_path: /assets/images/projects/receiptbox-screen-1.webp
    alt: "Instant Receipt Scanner & OCR"
    title: "On-Device OCR Scanner"
    excerpt: "Point your camera to extract merchant names, line items, dates, and total amounts in seconds with on-device OCR. Catch math errors and overcharges automatically."
  - image_path: /assets/images/projects/receiptbox-screen-2.webp
    alt: "Organized Expense Management"
    title: "Private Expense Management"
    excerpt: "Split bills proportionally, monitor spending categories, and generate tax-ready PDF or CSV exports with zero cloud servers or tracking."
gallery:
  - url: /assets/images/projects/receiptbox-screen-1.webp
    image_path: /assets/images/projects/receiptbox-screen-1.webp
    alt: "Instant Receipt Scanner & OCR"
  - url: /assets/images/projects/receiptbox-screen-2.webp
    image_path: /assets/images/projects/receiptbox-screen-2.webp
    alt: "Organized Expense Management"
categories:
  - software
tags:
  - Mobile
  - Finance
  - OCR
  - Expenses
  - Flutter
  - Offline-First
  - Privacy
---

I'd been keeping receipts in a folder for taxes and it was a mess. Photographing them still meant I had to type everything out manually, and the apps I tried wanted cloud access to my financial data.

**ReceiptBox** scans the receipt with your camera, pulls out the totals and line items on-device, and flags if the math doesn't add up. You can also split the bill with friends and export a clean report at tax time. Nothing leaves your phone.

## Key Features

{% include feature_row %}

* **Instant OCR Scanning**: Point your camera to extract merchant names, line items, dates, and total amounts in seconds using fast on-device optical character recognition.
* **Math Error & Overcharge Detection**: Automatically verifies that item subtotals, tax rates, and tips sum up accurately to the final charged total, catching merchant mistakes or accidental double charges.
* **Smart Bill Splitting**: Tap items to assign them to specific friends, calculate proportional tax and tip shares, and generate direct Venmo or Cash App payment requests.
* **Tax-Ready Export Reports**: Generate clean PDF reports with embedded receipt images, or export raw CSV/Excel spreadsheets formatted for tax filings and company reimbursements.
* **Visual Spending Insights & Budgets**: Monitor monthly spending with intuitive category breakdowns, set budget limits, and see exactly where your money goes.
* **100% Offline & Private**: Zero accounts, zero cloud servers, and zero telemetry. All scans and expense histories remain exclusively on your device.

## Screenshots

{% include gallery %}

## Tech Stack

* **Framework**: Flutter & Dart
* **OCR & Vision**: On-Device Optical Character Recognition (ML Kit)
* **Storage**: Local SQLite Database
* **Reporting**: PDF Document Generation & CSV Export
* **Platforms**: iOS (iPhone & iPad) & Android

{% include app-cta-box.html %}
