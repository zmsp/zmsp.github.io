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
App : [http://coronavirusdashboard.live/](http://coronavirusdashboard.live/)



# Why I built this?

I built this [web app](http://coronavirusdashboard.live/)  with the motivation of visualizing the data that's easy to read and user friendly. At the time of when I started building this webapp, there were not many relevent sources except JHU. My goal was to provide insights on coronavirus.

# Analytics 
Here are some insights on death rate, recovery rate and population infection rate by countries. 

<iframe width="600" height="450" src="https://datastudio.google.com/embed/reporting/8b0b2857-1f24-4e1f-b4e9-df7082dafe72/page/8sXIB" frameborder="0" style="border:0" allowfullscreen></iframe>

# Raw Data:
You can explore the raw data from here
* https://coronavirusdashboard.live/analysis/data.html
* https://github.com/zmsp/coronavirus-json-api/


## Data sources
The data is updated from Johns Hopkins University Center for Systems Science and Engineering [JHU CSSE](https://github.com/CSSEGISandData/COVID-19) repository and hosted on
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

