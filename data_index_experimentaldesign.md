---
  layout: default
permalink: /data/index/experimentaldesign
title: "Experimental Design"
---
  
  
# Experimental Deisgn
  
  [Data Science and Analytics Methods](https://benjburgess.github.io/data/index)

## Introduction

Most research is concerned with using experiments to answer a particular research question. Here, I provide a basic introduction to some of the most important questions that a researcher can ask about their experimental design and the choices that may need to be made to minimize resource costs, without compromising statistical power.

##Explanation

When designing an experiment (whether it be in biology, business, or any other field), it is crucial to ask the following question of: “*Is my experiment capable of answering my question?*” (Johnson et al., 2015). In some ways this question is obvious. For example, if conducting an A/B test to determine whether a promotion increased sales of a product, the A and B groups would need to be randomized (e.g., participant age, income, location, etc.), as if they weren’t, the results of this test might be misleading. 

In other ways, this question addresses issues which are perhaps less clear. For example, if the same A/B study was conducted twice, the first with 100 participants per group and the second with 10,000 participants per group, we would probably give a greater consideration to the results of the second study. In this example, we might implicitly decide that the results of the second study are ‘*more reliable*’ or ‘*more likely to be true*’ given the greater sample sizes. 
When designing experiments, one maxim that is often taught is ‘*the bigger (the sample size) the better*”. 
However, this is not necessarily true; although, experiments with overtly small sample sizes may not necessarily provide any actionable insights. Instead, there comes a point when increasing sample sizes will not provide any statistical benefit to an experiment. Let’s consider the following example. 

An agricultural company wants to know whether a particular fertilizer increases the yield of wheat in their fields. Given the financial cost of this new fertilizer, the company is only interested in using this new fertilizer if it has a moderate effect on increasing wheat yields compared to not using a fertilizer at all. As such, an A/B test is to be set up where the A group uses no fertilizer, and the B group trials the new fertilizer. However, what now needs to be determined is the sample sizes that should be used for each group. Every sample requires resources (time, labour, money, space, etc.) and so the company wants to design the study to minimize the resource costs without compromising the statistical power of the experiment. As such, what sample size should be used for the control and treatment groups?

At first, this question seems difficult to answer as we need to strike a balance between statistical power and the resource costs of the experiment. However, let’s start by thinking about how we would analyse any potential data from this study. When comparing between two groups (as we are doing here), there are a range of statistical tools we can use (e.g., t-test, ANOVA, response ratio etc.). For this example, we’re going to use *Hedges’ d* which is an effect size used to compare the means of two groups (Hedges, 1981). In brief, Hedges’ d comprises two parts, the effect size itself and associated confidence intervals. For interpreting Hedges’ d, if the effect size value is 0, then there is no difference between the two groups. Likewise, a rule of thumb for Hedges’ d, is that effect size values of 0.2, 0.5, and 0.8 correspond to small, medium, and large effects (i.e., differences between the two groups) respectively (Lakens, 2013). However, if the confidence intervals for the effect size overlap 0, then we don’t have a great deal of uncertainty in our results. This then means that we are unable to conclude that there is a difference in the means of our two groups. As with most statistical tests, increasing sample sizes increases the statistical power of the experiment and hence its ability to detect statistically smaller effects. Accordingly, for Hedges’ d, we would require a larger sample size to detect a statistically significant small effect, than we would to detect a statistically significant large effect.
  
If we head back to our example, we can see that the agricultural company is only interested in determining whether the new fertilizer has a moderate effect on increasing wheat yields. As such, using the above rule of thumb, we could design our experiment so that is capable of determining an effect size value (Hedges ‘d) of 0.5 or larger. Doing so would mean that we would be unable to detect a statistically significant small effect, but given the aims of the company and experiment, this is perfectly acceptable. Here, a Hedges’ d value of 0.5 can be referred to as our *critical effect size* (Mudge, 2013), in other words the minimum effect size that we need our experiment to be able to detect. Accordingly, we can now base our decisions on sample sizes around this critical effect size. Luckily, we can easily rework the mathematical equations for Hedges’ d, to determine required sample sizes based on a critical effect size. I’m not going to go into the mathematics behind this here (as it can get a little bit messy) but I will hopefully write a short tutorial on this soon. 

Overall, we can use the above method, to determine that by using sample sizes of **31** for each group in our experiment we will be able to detect whether the new fertilizer has a moderate (and statistically significant) effect on wheat yields. In doing so, we have determined the minimum sample size we should use for our experiment which minimizes resource (time, money, etc.) costs while maintaining the statistical power of our study. While we have based this example on a rule of thumb, in a real-world example we might be better off basing our choice of critical effect size on previously conducted experiments (Lakens, 2013).

Doing this analysis before we start our experiment is highly recommended, as otherwise we may only find out later on that we either invested unnecessary resources in our experiment, or that our experiment lacked the statistical power to answer our question (Lakens, 2021). This is one of the many questions which I attempted to tackle over the course of my PhD in computational ecology. While this is only a simple example, those I tackled in my PhD used more complex experimental designs (Burgess et al., 2021) but still attempted to determine how we can improve, or optimize, our studies to answer our research questions.



##References

Burgess, B. J., Jackson, M. C., & Murrell, D. J. (2021). Multiple stressor null models frequently fail to detect most interactions due to low statistical power. *bioRxiv*.

Hedges, L. V. (1981). Distribution theory for Glass's estimator of effect size and related estimators. *Journal of Educational Statistics*, 6(2), 107-128.

Johnson, P.C., Barry, S.J., Ferguson, H.M. and Müller, P. (2015). Power analysis for generalized linear mixed models in ecology and evolution. *Methods in Ecology and Evolution*, 6(2), 133-142.

Lakens, D. (2013). Calculating and reporting effect sizes to facilitate cumulative science: a practical primer for t-tests and ANOVAs. Frontiers in Psychology, 4, 863.

Lakens, D. (2021). Sample size justification. *psyarXiv*.

Mudge, J. F. (2013). Explicit consideration of critical effect sizes and costs of errors can improve decision-making in plant science. *New Phytologist*, 199(4), 876-878.

