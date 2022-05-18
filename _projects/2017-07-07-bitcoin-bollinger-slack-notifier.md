---
title:  "bitcoin-bollinger-slack-notifier"
excerpt: "Script that sends slack messages"
toc: true
categories:
- software
tags:
- API
- python
---


[![GitHub stars](https://img.shields.io/github/stars/zmsp/bitcoin-bollinger-slack-notifier?style=for-the-badge)](https://github.com/zmsp/bitcoin-bollinger-slack-notifier/stargazers)   
  

[![GitHub forks](https://img.shields.io/github/forks/zmsp/bitcoin-bollinger-slack-notifier?style=for-the-badge)](https://github.com/zmsp/bitcoin-bollinger-slack-notifier)  
  

Code repository: [bitcoin-bollinger-slack-notifier](https://github.com/zmsp/bitcoin-bollinger-slack-notifier)  

# The story: 
Bollinger Bands were created by John Bollinger in the 1980s as a way to measure market volatility. The idea is that when markets are more volatile, the bands will widen, and when markets are less volatile, the bands will narrow. Bollinger Bands are typically calculated using a 20-day moving average, with the upper and lower bands being 2 standard deviations above and below the moving average.

I was first introduced to Bollinger Bands when I was learning about machine learning for trading.

The code sends slack notification when it sees a buy or sell signal on bitcoin price. 