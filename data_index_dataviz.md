---
layout: default

permalink: /data/index/dataviz/
  
title: "Data Visualisation"
---
  
# Data Visualisation

[Data Science and Analytics Methods](https://benjburgess.github.io/data/index)

[Covid-19 Dashboard (Shiny)](https://benjburgess.shinyapps.io/covid19_utla_dashboard/)

[Covid-19 Dashboard (Tableau)](https://public.tableau.com/app/profile/ben.burgess/viz/Covid-19DashboardRegion_Age/Covid-19Dashboard?publish=yes)

With any analysis or dataset, one of the most important aspects to consider is how such information will be presented. While the in-text reporting of statistical measures (e.g., means, effect sizes, or p-values) may undoubtedly be important, in many cases presenting this information in a figure will provide readers or viewers with a easier (and more intutitive) understanding of any results or data.

Accordingly, while it is an often overlooked component of any analysis, data visualisation is highly important given that it is capable of providing efficient, quick, and detailed insights. In many cases (particularly with the advent of Big Data) it is simply impractical (or even impossible) to summarise complex datasets in text. For instance, it may be difficult to summarise the different patterns (across different groups) for time series data; however, displaying this data in a figure means that the viewer is much more likely to be able to grasp the nuances or patterns of any dataset. Furthermore, where data visualisations are interactive, the viewer may have the opportunity to explore new patterns which were previously overlooked. 

One example of a large scale multifaced dataset, is data openly available on [Covid-19 in the United Kingdom](https://coronavirus.data.gov.uk/). This constantly updating dataset provides information on case, death, and vaccination rates (amongst other metrics) which can subset according to geographic location, gender, or age (amongst other variables). Accordingly, this dataset contains a multitude of information which may be difficult to summarise in text, but can be more easily interpretted through visualisations.

As such, based upon this dataset, I have built two different interactive dashboards using either [Shiny (R)](https://benjburgess.shinyapps.io/covid19_utla_dashboard/) or [Tableau](https://public.tableau.com/app/profile/ben.burgess/viz/Covid-19DashboardRegion_Age/Covid-19Dashboard?publish=yes) to showcase the different ways in which this openly available dataset can be visualised. 

The [Tableau dashboard](https://public.tableau.com/app/profile/ben.burgess/viz/Covid-19DashboardRegion_Age/Covid-19Dashboard?publish=yes) visualises on Covid-19 case and death rates for different regions across England. The case and death rate data is then further stratified by age group. Overall, the dashboard is interactive, with users able to specify which age groups, dates, and regions they wish to view data for.

The [Shiny dashboard](https://benjburgess.shinyapps.io/covid19_utla_dashboard/) visualises data on Covid-19 vaccination, case, and death rates for lower tier local authorities in England (the smallest geographic scale for which data is available). Users of this dataset are able to select up to four different local authorities to compare across a user-specific data range. Each time the dashboard is loaded, it downloads data from the UK Government API, meaning that visualised data is that which is most recently available.

The R code to generate the Shiny dashbaord is openly available from [my github account](https://github.com/benjburgess/CovidDashboard).

Links to access the Covid-19 dashboards are at both the top and bottom of this page.

[Covid-19 Dashboard (Shiny)](https://benjburgess.shinyapps.io/covid19_utla_dashboard/)

[Covid-19 Dashboard (Tableau)](https://public.tableau.com/app/profile/ben.burgess/viz/Covid-19DashboardRegion_Age/Covid-19Dashboard?publish=yes)


