---
layout: handbook-page-toc
title: "Sample sizes for surveys"
description: "A guide to help determine your survey sample size."
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

In a perfect world, we’d sample every single user within the [population](https://statsandr.com/blog/what-is-the-difference-between-population-and-sample/).  However, we can’t do that. Why? It’s inefficient, expensive, time-consuming, and probably impossible to pull off.  Instead, we try to attain a _representative sample of the population_ from the population we want to focus on. To do this, we take a slice of that population, referred to as our ‘sample’. 

Furthermore, we compute measures from the sample and use them as _estimates of the measures_ for the entire population. For example, we can’t measure every users’ SUS score, even though that true SUS score does exist. Instead, we compute the SUS score from a sample of users. While it’s not going to be the exact SUS score for the population, it’s close within some degree of error (or margin of error). 

One of the most common questions around sampling is _‘how many people should we sample?’_  The correct answer is: _‘It depends’_. There are several factors to consider when determining how large your sample should be. The main factors we look at are: confidence/accuracy, population, and the type of analysis. Further, not all studies need a high level of accuracy, but the information is still very valuable/useful, allowing you to make informed decisions. Here’s what we mean:

- **Scenario 1:** If your research questions require a high degree of accuracy, such as a granular measure, you’ll want to sample more people. Example: SUS (n=200)
     - Why? SUS is measured over time, because we want to pick up on changes. When we see changes in SUS scores, we want to be confident that it is due to a true change and not because we were lucky or unlucky with our sampling. Smaller samples can be more sensitive to errors.
     - - SUS is measured across the entire population of users; therefore, we have a much larger pool of people to sample from. To ensure we have accuracy in the sample, we need a larger sample size. 
     - - Company-wide goals are set around SUS. Thus we want a high degree of accuracy. As the sample size increases, your error (or margin of error)—in other words, your likelihood of lucky or unlucky sampling—goes down, and the observations you make with your data are more accurate. 

- **Scenario 2:** If your research is trying to understand how many people are doing a certain workflow, or how people would rank certain features, you probably don’t need as many people to sample as the above Scenario 1. Example: survey to understand how users are ranking features (n=30)
     - - Why? Not all users use every workflow, so your population is not the entire GitLab user base. Rather, it’s all users of the workflow you are researching. A smaller population means you don’t need as large of a sample. 
     - - You are not collecting a measure that is being compared over time. In other words, the measure is not as granular compared to Scenario 1. 
     - - You don’t need a high level of accuracy to make a decision. Knowing from 30 users how they rank features is enough for you to make a confident decision. 

- **Scenario 3:** If your research is trying to understand what kinds of tools users’ incorporate in their workflow, you will likely have more open-ended questions in the survey. Example: survey to understand tools in a workflow (n=30)
     - - Why?  You don’t need as large of a sample for accuracy, since you are not computing a measure. Rather, you’re trying to get an idea of what responses users give. 
     - - You might be looking to target certain tools that users list and want to conduct follow up interviews to understand how they are using the tool. 
     - - A sample size of 30 is commonly used because that number is [large enough to accrue a normal distribution in scores even from populations where there is a skewed distribution](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5370305/). In short, this number helps us prevent bias in our results. 

To help make it easier to determine sample sizes, here are some guidelines:

- Ranking survey
     - Sample size target: 30
- Quantitative survey
     - Sample size target: 100
- Qualitative survey
     - Sample size target: 30

These are general guidelines, but the size will vary depending on your study and the  level of accuracy needed. You can use a [sample size calculator](https://www.qualtrics.com/blog/calculating-sample-size/), but you will need to know your population size. 

Not every result needs to be statistically significant. You can sometimes gather enough responses to have meaningful inferences while not achieving statistical significance. What’s more important is to have a representative sample of the population of interest. 
