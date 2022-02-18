---
layout: default

permalink: /data/index/nma/
  
title: "Network Meta-analyses"
---
  
# Network Meta-analyses
  
[Data Science and Analytics Methods](https://benjburgess.github.io/data/index)

## Introduction

Meta-analyses are a powerful statistical technique which are commonplace in a variety of fields such as medicine, psychology, and ecology. Indeed, over the course of my PhD in Computational Ecology I've spent a lot of time working on meta-analyses of multiple stressors (e.g., [Burgess et al., 2021](https://onlinelibrary.wiley.com/doi/full/10.1111/gcb.15630)). In short meta-analyses work by collating data from multiple different scientific papers which all address the same question. These datasets are then analysed in a standardised manner with the results of these different studies then being collating into a single metric which is used to identify trends in what is often complex datasets. Meta-analyses can be quite convoluted to conduct; however, meta-analysis have a greater statistical power than any of the individual studies from which they collate data and as such their findings can have high statistical power and (if conducted properly) provide valuable insights (e.g., vaccine safety; [Taylor et al., 2014](https://www.sciencedirect.com/science/article/pii/S0264410X14006367)).

Meta-analyses can take many different forms. For instance, meta-analyses may be bayesian or frequentist in nature. Similarly, meta-analyses may be simply pairwise or consider an entire network. For instance, the below figure illustrates an example of an pairwise meta-analysis, namely there are two treatment groups which are compared (Placebo and Metformin 2000mg).

<div style="text-align:center"><img src="https://benjburgess.github.io/assets/example_pma.jpeg" width="50%"/></div>

In contrast, network meta-analyses can contain may different groups and have a complex network structure. For example, the below figure illustrates an example of a relatively simple network meta-analysis where there are nine different treatment groups which are compared (e.g., Placebo, Metformin 2000mg, Sotagliflozin 200mg, etc.).

<div style="text-align:center"><img src="https://benjburgess.github.io/assets/example_nma.jpeg" width="50%"/></div>