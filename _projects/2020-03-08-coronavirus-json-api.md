---
title: "Coronavirus JSON API"
excerpt: "COVID statistics automatically pulled and served via JSON"
header:
  teaser: /assets/images/projects/placeholder_large.jpeg
toc: true
categories:
  - software
tags:
  - Data
  - API
  - Automation
---

[![GitHub stars](https://img.shields.io/github/stars/zmsp/coronavirus-json-api?style=for-the-badge)](https://github.com/zmsp/coronavirus-json-api/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/zmsp/coronavirus-json-api?style=for-the-badge)](https://github.com/zmsp/coronavirus-json-api)

An automated API that pulls COVID-19 statistics hourly from JHU and Worldometers, producing JSON data for easy consumption by other tools.

## The Story

When the COVID-19 pandemic first started, the World Health Organization released its data. JHU held the data in a GitHub repository. However, there was no good way to access the data initially. So, I created some scripts to pull CSV data hourly from the JHU data repository and produce JSON data that could be consumed by other tools.

The JSON files were committed to a GitHub repo which allowed anyone to link their app to this data without using any 3rd party service. I used the same data API to build zobairshahadat.com/coronavirus/.

## Data Sources

- **Primary Source**: Johns Hopkins University Center for Systems Science and Engineering ([JHU CSSE](https://github.com/CSSEGISandData/COVID-19)).
- **Real-time Totals**: Updated every hour from [Worldometers](https://www.worldometers.info/).

The project is now dormant as there are many alternative APIs available.

## Links

- **Source Code**: [GitHub Repository](https://github.com/zmsp/coronavirus-json-api)
