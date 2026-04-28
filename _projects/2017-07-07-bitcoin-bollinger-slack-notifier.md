---
title: "Bitcoin Bollinger Slack Notifier"
excerpt: "Script that sends Slack messages for Bitcoin trading signals"
header:
  teaser: /assets/images/projects/bitcoin-bollinger-slack-notifier.jpg
sidebar:
  - title: "Repository"
    text: "[![GitHub stars](https://img.shields.io/github/stars/zmsp/bitcoin-bollinger-slack-notifier?style=for-the-badge)](https://github.com/zmsp/bitcoin-bollinger-slack-notifier/stargazers)  \n[![GitHub forks](https://img.shields.io/github/forks/zmsp/bitcoin-bollinger-slack-notifier?style=for-the-badge)](https://github.com/zmsp/bitcoin-bollinger-slack-notifier)"
toc: true
categories:
  - software
tags:
  - API
  - python
---

A Python script that sends Slack notifications when it detects a buy or sell signal for Bitcoin based on Bollinger Bands.

## The Story

Bollinger Bands were created by John Bollinger in the 1980s as a way to measure market volatility. The idea is that when markets are more volatile, the bands will widen, and when markets are less volatile, the bands will narrow. Bollinger Bands are typically calculated using a 20-day moving average, with the upper and lower bands being 2 standard deviations above and below the moving average.

I was first introduced to Bollinger Bands when I was learning about machine learning for trading.

## Links

- **Source Code**: [GitHub Repository](https://github.com/zmsp/bitcoin-bollinger-slack-notifier)