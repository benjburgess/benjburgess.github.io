---
layout: default
permalink: /data/index/metaanalyses
title: "Meta-Analyses"
---
  
  
# Meta-analyses
  
[Data Science and Analytics Examples](https://benjburgess.github.io/data/index)

## Introduction

[Introductory Meta-analysis Tutorial](https://benjburgess.github.io/i/metaanalysis_introductory)

Meta-analyses are a powerful statistical technique which are commonplace in a variety of fields such as medicine, psychology, and ecology. Indeed, over the course of my PhD in Computational Ecology I've spent a lot of time working on meta-analyses of multiple stressors (e.g., [Burgess et al., 2021](https://onlinelibrary.wiley.com/doi/full/10.1111/gcb.15630)). In short meta-analyses work by collating data from multiple different scientific papers which all address the same question. These datasets are then analysed in a standardised manner with the results of these different studies then being collating into a single metric which is used to identify trends in what is often complex datasets. Meta-analysis can be quite convoluted to conduct; however, meta-analysis have a greater statistical power than any of the individual studies from which they collate data and as such their findings can have high statistical power and (if conducted properly) provide valuable insights (e.g., vaccine safety [(Taylor et al., 2014)](https://www.sciencedirect.com/science/article/pii/S0264410X14006367)). However, there are numerous pitfalls which meta-analysts can fall into (some obvious and some less so) and ensuring the methodological rigour of meta-analyses is essential.


## Meta-analyses - R Tutorial

There are a number of fantastic resources on meta-analysis which go through the basic theory underpinning this statistical method (see the links at the end of this page). As such, I've focussed on developing some examples of how to implement meta-analyses in R. Here, I've written a thorough tutorial, with a relatively complex dataset, which illustrates how to conduct a meta-analysis which is statistically rigourous. 


### Introductory Tutorial

An [introductory tutorial for meta-analyses](https://benjburgess.github.io/i/metaanalysis_introductory) where `R` code is provided. The tutorial provides a step-by-step workflow for how to conduct a meta-analysis including addressing issues with covariance, hierarchical random effects, and fixed effects.



## Introductory Explanations of meta-analyses

[Nature (Gurevitch et al., 2018)](https://www.nature.com/articles/nature25753)

[BMJ (Shorten & Shorten, 2013)](https://ebn.bmj.com/content/16/1/3)

[metafor (Viechtbauer, 2010)](https://www.metafor-project.org/doku.php)