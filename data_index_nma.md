---
layout: default

permalink: /data/index/nma/
  
title: "Network Meta-analyses"
---
  
# Network Meta-analyses
  
[Data Science and Analytics Methods](https://benjburgess.github.io/data/index)

[WINBUGS to R: Replicating a published Bayesian Network Meta-analysis in R](https://benjburgess.github.io/i/nma_bayesian)

## Introduction

Meta-analyses are a powerful statistical technique which are commonplace in a variety of fields such as medicine, psychology, and ecology. Indeed, over the course of my PhD in Computational Ecology I've spent a lot of time working on meta-analyses of multiple stressors (e.g., [Burgess et al., 2021](https://onlinelibrary.wiley.com/doi/full/10.1111/gcb.15630)). In short meta-analyses collate data from multiple different studies which all address the same question. These datasets are analysed in a standardised manner with the results of these different studies then being collating into a single metric which is used to identify trends in complex datasets. Meta-analyses can be quite convoluted to conduct; however, meta-analysis have a greater statistical power than any of the individual studies from which they collate data and as such their findings can have high statistical power and (if conducted properly) provide valuable insights (e.g., vaccine safety; [Taylor et al., 2014](https://www.sciencedirect.com/science/article/pii/S0264410X14006367)).

Meta-analyses can take many different forms; for instance, meta-analyses may be bayesian or frequentist in nature. Similarly, meta-analyses may be simply pairwise or consider an entire network. For instance, the below figure illustrates an example of an pairwise meta-analysis, namely there are two treatment groups which are compared (Placebo and Metformin 2000mg).

<div style="text-align:center"><img src="https://benjburgess.github.io/assets/example_pma.jpeg" width="60%"/></div>

In contrast, network meta-analyses can contain may different groups and have a complex network structure. For example, the below figure illustrates an example of a relatively simple network meta-analysis where there are nine different treatment groups which are able to be compared (e.g., Placebo, Metformin 2000mg, Sotagliflozin 200mg, etc.).

<div style="text-align:center"><img src="https://benjburgess.github.io/assets/example_nma.jpeg" width="60%"/></div>

One of the strengths of the network meta-analysis is that groups for which there is no direct comparison are able to be indirectly compared. For instance, in the above network plot, a network meta-analysis would allow for Dapagliflozin (5mg) to be compared to Sotagliflozin (400mg) given that they can be connected via the Placebo treatment group.

To demonstrate network meta-analyses, I've compiled a [tutorial which replicates the Bayesian network meta-analysis from a recently published paper](https://benjburgess.github.io/i/nma_bayesian) by [Langford et al. (2020)](https://dom-pubs.onlinelibrary.wiley.com/doi/10.1111/dom.13863). The original analysis by Langford et al. (2020) was conducted using WINBUGS. However, I have been able to exactly replicate their results using the gemtc package in R. This tutorial aims to provide an introduction to Bayesian network meta-analyses in R using a real world dataset.

