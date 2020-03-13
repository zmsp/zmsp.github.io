---
title:  "Coronavirus webapp development"
header:
  teaser: https://i.imgur.com/khtGild.png
  og_image: https://i.imgur.com/khtGild.png
  overlay_image: https://i.imgur.com/khtGild.png
categories:
  - datascience
tags:
  - data
  - analytics
  - visualization
  

---


# This page documents the motivation and the process behind building a webapp using COVID-19 data. 
App : [coronavirus2020.icu](http://www.coronavirus2020.icu)



# Why I built this?

I built this [web app](http://coronavirusdashboard.live/)  with the motivation of visualizing the data that's easy to read and user friendly.





## Data sources
The data is updated from Johns Hopkins University Center for Systems Science and Engineering (JHU CSSE) repository and hosted on
https://github.com/zmsp/coronavirus-json-api/


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
Borrowed some ideas form Material Design Philosophy. Flutter widgets provide some ready to use interfaces that's aesthetically pleasing. 


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

