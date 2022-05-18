---
title:  "coronavirus json api"
excerpt: "COVID statistics automatically pulled"
header:
  teaser: https://i.imgur.com/khtGild.png
  og_image: https://i.imgur.com/khtGild.png
  overlay_image: https://i.imgur.com/khtGild.png
categories:

- software 
  
tags:
- data
- analytics
- visualization
- python

---






## Code:

[![GitHub stars](https://img.shields.io/github/stars/zmsp/coronavirus-json-api?style=for-the-badge)](https://github.com/zmsp/coronavirus-json-api/stargazers)   
  

[![GitHub forks](https://img.shields.io/github/forks/zmsp/coronavirus-json-api?style=for-the-badge)](https://github.com/zmsp/coronavirus-json-api)  
  

Code repository: [coronavirus-json-api](https://github.com/zmsp/coronavirus-json-api)  


## The story

When the COVID-19 pandemic first started, the World Health Organization released it's data. JHU hold the data in a github repository. However, there were no good way to access the data initially. So, I created some scripts to pull csv data hourly from JHU data repository, and produce json data that could be consumed by other tools.

The JSON files were commited in a github repo which would allow anyone to link their app to these data without using any 3RD party service. 


I used the same data API to build coronavirusdashboard.live which was recently replaced and moved to zobairshahadat.com/coronavirus/

## Purpose:

The project was used to serve ase API backend for https://zmsp.github.io/coronavirus
During the start of COVID-19 pandemic, I wanted to create a site that services as a window to covid statistics.

## Data sources

The data is updated from Johns Hopkins University Center for Systems Science and
Engineering [JHU CSSE](https://github.com/CSSEGISandData/COVID-19) repository and hosted on
https://github.com/zmsp/coronavirus-json-api/ JHU CSSE updates the data about twice daily.

Additionally, the total counts are updated every hour from https://www.worldometers.info/

The project is now dormant a there are many alternative APIs avaiable. 


