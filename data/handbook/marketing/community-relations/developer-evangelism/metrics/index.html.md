---
layout: handbook-page-toc
title: "Metrics Collection & Analysis"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}


## Team Impressions

### 2021 Twitter Impressions

![Dev Evangelism 2021 Impressions](https://europe-west1-group-community-a29572.cloudfunctions.net/getKeyHoleData?grouping=group&grouping_data=de&datatype=impressions&year=2021&month=all&network=twitter&response_type=chart&chart_type=bar "Dev Evangelism 2021 Impressions")

### 2020 Twitter Impressions

![Dev Evangelism 2020 Impressions](https://europe-west1-group-community-a29572.cloudfunctions.net/getKeyHoleData?grouping=group&grouping_data=de&datatype=impressions&year=2020&month=all&network=twitter&response_type=chart&chart_type=bar "Dev Evangelism 2020 Impressions")


## Metrics Collections    

We currently collect ***ONLY*** Twitter impressions and YouTube video views using KeyHole.co and the YouTube API respectively, which are then fed into Sisense and other internal reporting platforms like Data Studio. Impressions on blog posts created on the GitLab blog are collected using Google Analytics. Impressions on blog posts prior to May 2021 are provided by Big Query. 

**Team members who consent to use KeyHole understand that these metrics are used only to measure team results and that they can opt out at any time.** Most of the activities of the team is centered around Twitter, that is why it forms the bulk of the team's metrics collection. We might consider metrics from other platforms used by the team as data collection and API access gets easier.

It is currently not possible to track metrics for LinkedIn personal profiles. Performance metrics for LinkedIn personal profiles that are used to determine performance required significant manual work to produce. Please note this as you review social performance data, that we are unable to quantify metrics for one of our two biggest channels.

## Tools

- [KeyHole](/handbook/marketing/community-relations/developer-evangelism/tools/keyhole/): Twitter Impressions/Engagements 
- [DE-Bot](https://gitlab.com/gitlab-com/marketing/corporate_marketing/developer-evangelism/code/de-bot):  Internal tool for issue triage and team workflow automation
- [DE-Dashboard](https://gitlab.com/gitlab-com/marketing/corporate_marketing/developer-evangelism/code/de-dashboard/): Internal tool for data collection and reporting.
- [Developer Evangelism Dashboard](https://datastudio.google.com/u/0/reporting/4cd1e6a9-23f2-4de1-b8fa-29e42cb646c1/page/YsgmB): Holistic view of all metrics collected for the Evangelist Program.
- [Requests Impression Tracker Sheet](https://docs.google.com/spreadsheets/d/10E_TagnV6xgjHorWPTpMnO1Qk33lPR9HkGHOJfa0ENM/edit#gid=1283634798)


## DE Dashboard

The [DE-Dashboard](https://gitlab.com/gitlab-com/marketing/corporate_marketing/developer-evangelism/code/de-dashboard/) is a GitLab Pages project, which serves as a central point for all data collection. It serves the following purposes:
  - [Retrieve list of DE Youtube videos](https://gitlab.com/gitlab-com/marketing/corporate_marketing/developer-evangelism/code/de-dashboard/-/blob/master/youtube.rb) to Google Sheet for tracking
  - Analyze Developer Evangelism issue creation and closure in the Corporate marketing issue tracker
  - Host the data endpoint for Social media metrics
  - Computation and report of [team request budgets](/handbook/marketing/community-relations/developer-evangelism/). 
