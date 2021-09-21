---
layout: default

permalink: /Covid19/
  
title: "Covid-19 Dashboard"
---
  
# Covid-19 Dashboard

[Covid-19 Dashboard](https://benjburgess.shinyapps.io/coviddashboard/)



Since the start of the Covid-19 pandemic in March 2020, it has been apparent that the occurrence and spread of the virus is not geographically uniform. In England this has been seen with places such as Leicester and Manchester being placed under strignet restrictions at various points in 2020, while other areas were under less strict measures. 

Such geographic disparities have also been evident with the rise of new Covid variants. In the winter of 2020/2021 the alpha variant (formerly known as the Kent variant) spread out from south-eastern England towards other areas of the UK (e.g., northern England and the Midlands). This spread was likewise accompanied by a tiered system of restrictions being implemented across England.

Case and death rates of Covid-19 have fluctated, with this due to the transmissibility of different variants (e.g., alpha, delta), the implementation of restrictions (e.g., social distancing), and the roll-out of vaccinations. As such, the prevalence of Covid-19 has varied both geographically and temporally.

The UK Government provides an interesting dashboard (https://coronavirus.data.gov.uk/details/) with the ability to breakdown various measures and statistics by different localities. However, it does not easily allow for comparisons of the same metric (e.g. number of cases) across time for multiple different locations. Accordingly, given that these comparisons are not easy to make using the UK Government's own dashboard, I built [my own dashboard](https://benjburgess.shinyapps.io/coviddashboard/) (written in R using Shiny) which allows such comparisons to be made.

[The dashboard](https://benjburgess.shinyapps.io/coviddashboard/) uses data freely available from the UK Government (under Open Government License v3.0) and automatically updates every time the dashboard is launched. Data is provided on the number of cases, the number of deaths, and the proportion of people who have been fully vaccinated. Data is available from 01/11/2020 onwards and up to four different lower tier local authorities (e.g., Westminster, County Durham, Wyre Forest) are able to be compared. Dates for which data are shown are also able to be selected by the user.

The R code to generate this dashbaord is openly available from [my github account](github.com/benjburgess).

Links to access the Covid-19 dashboard are at both the top and bottom of this page.

[Covid-19 Dashboard](https://benjburgess.shinyapps.io/coviddashboard/)

