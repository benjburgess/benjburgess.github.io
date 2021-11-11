---
layout: default

permalink: /multiplestressR/
  
title: "multiplestressR"
---
  
# *multiplestressR* - R Package
  
<div style="text-align:center"><img src="https://benjburgess.github.io/assets/multiplestressR_Fig.jpg" width="100%"/></div>
<br />  
  
My time as a PhD student in computational ecology was spent using various different computational and statistical approaches to better understand how stressors (e.g., climate change, pollution, or invasive species) interact to affect ecosystems. The field of multiple stressor ecology has greatly expanded from the dozen or so papers published at the turn of the century and is continuing to grow every year. Many, if not most, of the papers in the field attempt to understand these stressors interact using null models which then allow interactions to be classified as either a *null*, *antagonistic*, *synergistic* or *reversal* interaction.

However, one of the major difficulties facing the field is that most of the highly cited papers implement statistical methods (i.e., null models) that differ from one another (sometimes a only little bit, other times to a large degree). As such, it can be difficult to know when results are due to ecological factors or differences in methodology.

In an attempt to remove these methodological differences, I have written an R package called *multiplestressR* which allows researchers to conduct a thorough statistical analysis of their data in just a few lines of code. The functions in *multiplestressR* have been written so as to be accessible to anyone regardless of their knowledge of either R or the statistical null models which are commonly implemented in multiple stressor ecology. Indeed, researchers can select whether to implement the additive or multiplicative null model on their dataset and then classify individual interactions. Furthermore, the package can then generate summary figures which can help the researcher interpret their analyses (see the above figure).

The *multiplestressR* package is applicable to anyone using null models to classify interactions from individual experiments through to meta-analyses. As such, the hope is that by using a single, consistent, rigourous framework to classify interactions, studies can be more easily compared. As such any differences between these studies can hence be attributed to ecological or environmental factors and not methodological differences.

The *multiplestressR* package is available from [CRAN (where full technical details of the package can be found)](https://cran.r-project.org/package=multiplestressR) and can be installed in R using the following code:

```
install.packages("multiplestressR")
```

I have also put together an [introductory tutorial](https://benjburgess.github.io/i/multiplestressR1) on the *multiplestressR* package, showcasing how an analysis can be conducted using the package.


