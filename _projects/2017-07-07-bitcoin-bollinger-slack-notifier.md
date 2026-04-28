---
title: "Bitcoin Bollinger Slack Notifier"
excerpt: "Slack messages for Bitcoin trading signals"
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

I made this while learning about machine learning for trading. It's a simple Python script that pings Slack whenever Bollinger Bands suggest a buy or sell signal for Bitcoin.

## How it works
Bollinger Bands measure market volatility. When the price hits the upper or lower bands (2 standard deviations from the 20-day moving average), the script triggers a notification so I don't have to keep an eye on the charts all day.

## Links
- **Source Code**: [GitHub Repository](https://github.com/zmsp/bitcoin-bollinger-slack-notifier)