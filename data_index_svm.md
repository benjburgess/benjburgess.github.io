---
layout: default
permalink: /data/index/svm
title: "Support Vector Machines"
---
  
  
# Support Vector Machines
  
[Data Science and Analytics Examples](https://benjburgess.github.io/data/index)

## Introduction

[Introductory SVM Tutorial](https://benjburgess.github.io/i/SVM_linear)

[Advanced SVM Tutorial](https://benjburgess.github.io/i/SVM_radial)

Support vector machines (SVMs) are one of the most popular machine learning methods which are used to classify data into two or more groups. Indeed, SVMs have a myriad of different applications from genetics through to the classification of different facial expressions. SVMs represent a supervised machine learning approach, namely they require training before they can be used to classify datasets. However, while a commonplace method, SVMs are relatively complex requiring users to make a number of decisions. For instance, users must first ensure that their data is in the appropriate format (i.e., cleaned and standardised) and not biased towards a given class or group. Likewise, SVMs require decisions about which kernel to implement (alongside other potential parameter choices). For example, choosing a *linear* kernel as opposed to *radial* kernel may greatly alter the accuracy of any SVM. Indeed choice of which SVM kernel to use may require an understanding of your dataset.


## Support Vector Machine - R Tutorials

There are a great many resources which either go through the basic theory or explanations of SVMs (see the links at the end of this page). As such, rather than re-invent the wheel, I've focussed on putting together some examples of how to implement SVMs in R. Here, I've written two tutorials, one with a very simple dataset, and one with a more complex dataset which illustrates some of the potential limitations of SVMs. These are described more below.


### Introductory Tutorial

The [introductory tutorial](https://benjburgess.github.io/i/SVM_linear) builds a simple SVM capable of accurately classifying two different species based on data for their heights and weights. This provides an example of how to implement an SVM in R, and some basic examples of data cleaning which is required prior to any analysis.

### Advanced Tutorial

The [advanced tutorial](https://benjburgess.github.io/i/SVM_radial) builds a more complex SVM which attempts to classify wines into different quality classes based upon chemical data for each wine. This tutorial outlines some more advanced data cleaning (e.g., SCUT) and management (e.g., PCA) and the different measures by which SVM performance can be assessed.


## Introductory Explanations of SVMs

[Statquest](https://www.youtube.com/watch?v=efR1C6CvhmE)

[Towards Data Science (I)](https://towardsdatascience.com/support-vector-machine-introduction-to-machine-learning-algorithms-934a444fca47)

[Towards Data Science (II)](https://towardsdatascience.com/support-vector-machines-svm-c9ef22815589)