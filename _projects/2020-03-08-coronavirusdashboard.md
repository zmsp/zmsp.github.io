---
title:  "coronavirus dashboard"
excerpt: "Dashboard visualizing COVID spreads"
toc: true
categories:
- software

tags:
- data
- analytics
- visualization
- flutter

---

[![GitHub stars](https://img.shields.io/github/stars/zmsp/coronavirusdashboard?style=for-the-badge)](https://github.com/zmsp/coronavirusdashboard/stargazers)   
  

[![GitHub forks](https://img.shields.io/github/forks/zmsp/coronavirusdashboard?style=for-the-badge)](https://github.com/zmsp/coronavirusdashboard)  
  

Code repository: [coronavirusdashboard](https://github.com/zmsp/coronavirusdashboard)  




# This page documents the motivation and the process behind building a webapp using COVID-19 data.

App : [http://coronavirusdashboard.live/](http://zmsp.github.io/coronavirus)

# Code

If you are here for the code, its visible on this
repository https://github.com/zmsp/coronavirusdashboard/tree/master/flutter_code

# Why I built this?

I built this [web app](http://coronavirusdashboard.live/)  with the motivation of visualizing the data that's easy to
read and user friendly. At the time of when I started building this webapp, there were not many relevent sources except
JHU. My goal was to provide insights on coronavirus and help people with information.

# Analytics

Here are some insights on death rate, recovery rate and population infection rate by countries.

<iframe width="800" height="650" src="https://datastudio.google.com/embed/reporting/8b0b2857-1f24-4e1f-b4e9-df7082dafe72/page/8sXIB" frameborder="0" style="border:0" allowfullscreen></iframe>

# Raw Data:

You can explore the raw data from here
<iframe width="800" height="650" src="https://datastudio.google.com/embed/reporting/b9437400-6abc-431e-a608-cdbb988fa6a8/page/tzXIB" frameborder="0" style="border:0" allowfullscreen></iframe>

## Data sources

The data is updated from Johns Hopkins University Center for Systems Science and
Engineering [JHU CSSE](https://github.com/CSSEGISandData/COVID-19) repository and hosted on
https://github.com/zmsp/coronavirus-json-api/ JHU CSSE updates the data about twice daily.

Additionally, the total counts are updated every hour from https://www.worldometers.info/

## Tech Stack

* Flutter Web
* Github pages
* Python
* Numpy
* Pandas
* Google Maps API
* FontAwesome
* Windows.bat scripts

## Designing the User Interface

Borrowed some ideas form Material Design Philosophy. Flutter widgets provide some ready to use interfaces that's
aesthetically pleasing.

## issues faced while building

* The data source needed to be normalized as there were some missing values.
* The UI framework, flutter web, is still a beta product. I had to use a nontraditional way of implementing maps.
* The UI needed to be tuned to be used in desktop and mobiles. Making it universally compatible was a challenge.

## Future Plans

* Add map plot (added 3/8)
* Add time-series data  (3/10)
* Look into more data sources
* Improve upon UI
* Attempt to build an android app using the same source.
* Add statistics by demography

## Project timeline

* 3/6, built the API
* 3/7, finished creating an initial site.
* 3/8, added Google Map plot for coronavirus data
* 3/10 Add time-series data
* 3/12Incorporated external dashboards

