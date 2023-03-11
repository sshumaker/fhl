---
layout: handbook-page-toc
title: Crash Course for Product Stage Resources
---

## On this page
{:.no_toc}

- TOC
{:toc}


## Objectives for this page

This page is intended to provide a crash course style overview of the most important Product Analytics related resources for each product Stage.
As a Product Analyst or other curious GitLab team member, it can be helpful to have a quick and easy reference for each product Stage to quickly understand high-level functionality, key objectives or a distilled product roadmap, and key data resources currently used under a specific Stage or Group within GitLab before jumping in to an analysis.

If this page serves it's purpose, Product Analysts should be able to visit this handbook page before working with a Stage or Group to obtain helpful contextual information without needing to do a scavenger hunt search across dozens of handbook pages to find relevant information. 

## Helpful places to start

* [Internal handbook performance indicators (PIs)](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/) - This internal handbook page is a great place to understand the PIs for each Stage / Group to understand what results each team is trying to acheive.

* [Sisense Usage Insights](https://app.periscopedata.com/app/gitlab/1013112/Sisense-Usage-Insights) is a Dashboard that provides a high level analysis of most commonly used Sisesnse Dashboards, Data Sources, and Snippets.

* [Product categories handbook page](/handbook/product/categories/) contains a huge amount of helpful information and defines sections, stages, groups, and categories.

* Need to quickly learn how a certain Stage/Group feature works? [GitLab Docs](https://docs.gitlab.com/)

* [Metrics dictionary](https://metrics.gitlab.com/) contains metrics and events collected in Service Ping and Snowplow. For more information visit the dedicated [Product Intelligence Guide](/handbook/product/product-intelligence-guide/#metrics-dictionary).

* [Features by Group handbook page](/handbook/product/categories/features/#planproject-management-group) contains a tabular breakdown of features included in each Stage Group by Core, Premium or Ultimate categories. 

* [Definitive guides to data subject areas](https://about.gitlab.com/handbook/business-technology/data-team/data-catalog/#definitive-guides) managed by the Data team. 

* [Centralized SMAU/GMAU Dashboard](https://app.periscopedata.com/app/gitlab/758607/Centralized-SMAU-GMAU-Dashboard) contains CMAU, SMAU, and GMAU charts for each section, stage, and group.

* The [Technical Marketing handbook page](/handbook/marketing/brand-and-product-marketing/product-and-solution-marketing/technical-marketing/) contains links to product demos, webinars and release videos.  

* GitLab's Fiscal Year runs from February 1 to January 31. [Here](https://about.gitlab.com/handbook/finance/#fiscal-year) is a link to GitLab's Fiscal Quarter to Month map.

## Learn about analytics relevant product stage topics grouped by Section

Why are these groupings called 'Stages'? At GitLab, we build a product that supports every **stage** of the DevOps Lifecycle.

### Dev Section

#### Manage Stage
This Stage helps teams manage their software delivery lifecycle with metrics and value stream insight in order to streamline and increase their delivery velocity. Insights, authentication, audits, compliance, user management, group & sub-group management, and project management.

<details markdown="1"><summary>Click to expand</summary>


**Top dashboards referenced by this team**

* [Centralized SMAU/GMAU](https://app.periscopedata.com/app/gitlab/758607/Centralized-SMAU-GMAU-Dashboard)  Overall SMAU/GMAU dashboard primarily utilized by the Import Group

* [Manage Stage Sisense Topics Page](https://app.periscopedata.com/app/gitlab/topic/Manage-Stage/ab937816bcd24c9291ceb7b6c5e30c49)  Overall Manage stage pinned dashboards for easy access

* [Manage : Compliance](https://app.periscopedata.com/app/gitlab/663045/Manage:-Compliance-Dashboard)  Dashboard frequently used by the Compliance Group

* [Manage : Optimize Feature Usage](https://app.periscopedata.com/app/gitlab/779829/Manage:Optimize-Feature-Usage)  Dashboard frequently used by the Optimize Group


**Important data documentation**

``` sql

SELECT * 
FROM table
WHERE field = stage_name
;
```

**Helpful video resources**

[Plan:Optimize YouTube Channel](https://www.youtube.com/playlist?list=PL05JrBw4t0KopcuINFaWBEHYlaDnbDxpl)

Team meetings, AMAs, etc. for the Plan:Optimize Group

[Manage:Access YouTube Channel](https://www.youtube.com/playlist?list=PL05JrBw4t0Kot4GcDlWPsZOM8YgncnPUi)

Team meetings, AMAs, etc. for the Manage:Access Group

[Manage:Organization YouTube Channel](https://www.youtube.com/playlist?list=PL05JrBw4t0Kq-9cR2cz4uxUIfVYtB4Gq8)

Team meetings, AMAs, etc. for the Manage:Organization Group

**Product direction**

[Problems to Solve from Product Direction Page](https://about.gitlab.com/direction/manage/#problems-to-solve)

The Problems to Solve section of Manage's Product Direction Page is the most condensed documentation to understand Manage's big picture focus quickly.

**Performance indicators**

[Metrics from Product Direction Page](https://about.gitlab.com/direction/manage/#metrics)

This link breaks down the performance indicators for each Manage Group clearly and links out to the Internal Handbook PI page. 

**Key handbook pages**

[Manage Direction Page](https://about.gitlab.com/direction/manage/)

[Main Manage Stage Page](https://about.gitlab.com/handbook/engineering/development/dev/manage/)

**Slack channels**

**#s_manage**

**Team members**

[Handbook page to find Manage team members to collaborate with](/handbook/product/categories/#manage-stage)

</details>

#### Plan Stage
Enable teams to effectively plan and execute work in a single application. This stage enables portfolio planning and management through epics, groups (programs), milestones, etc. to organize and track progress

<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Plan xMAU (monthly)](https://app.periscopedata.com/app/gitlab/775807/Plan-xMAU-(monthly))  Overall Plan Stage xMAU dashboard

* [Centralized SMAU/GMAU](https://app.periscopedata.com/app/gitlab/758607/Centralized-SMAU-GMAU-Dashboard)  Most Group PMs on Plan utilize the Centralized SMAU/GMAU dashboard

* [Plan stage .com events](https://app.periscopedata.com/app/gitlab/654183/Plan-stage-.com-events)  Analyses dealing with Snowplow events tables

* [Say Do Ratios](https://app.periscopedata.com/app/gitlab/658030/Say-Do-Ratios)  Primarily engineering analytics utilized for Plan Stage decision making

* [Plan stage capacity planning](https://app.periscopedata.com/app/gitlab/587512/Plan-stage-capacity-planning)  Primarily engineering analytics utilized for Plan Stage decision making

**Important data documentation**

``` sql

SELECT * 
FROM table
WHERE field = stage_name
;
```

**Helpful video resources**

[Plan Stage YouTube playlist](https://www.youtube.com/playlist?list=PL05JrBw4t0KoceqcTneOVmAzhEp6NinY0)

**What the Plan Stage team is working on**

[Link to 1 Year Plan](https://about.gitlab.com/direction/plan/#1-year-plan)

A great handbook page to skim to understand the roadmap and focus for Plan

**Performance indicators**

[Link to performance indicators](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/product/dev-section/)

Resource to understand the Performance Indicators for the Dev Section - Page can be searched by Stage and Group

**Key handbook pages**

[Main Plan page](https://about.gitlab.com/handbook/product/categories/#plan-stage)

[Plan direction page](https://about.gitlab.com/direction/plan/)


**Slack channels**

**#s_plan**

**Team members**

[Handbook page to find Plan team members to collaborate with](/handbook/product/categories/#plan-stage)

</details>

#### Create Stage
Create provides tools that support the beginning of the DevOps Life Cycle. Source Code management, Code Review, Wiki, Web IDE, etc.

[Start on the GitLab website page](https://about.gitlab.com/features/) dedicated to Create to get an understanding of features included in this Stage. 

<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Create - Code Review Topics page](https://app.periscopedata.com/app/gitlab/topic/Create---Code-Review/abb4786159ef4aa7abad4da4c21b0871)  Create : Code Review group specific pinned dashboards for easy access

* [Code Review MAU Metrics](https://app.periscopedata.com/app/gitlab/786738/Code-Review-MAU-Metrics)  Used frequently by Create : Code Review Group

* [Editor Extension Category MAU Metrics](https://app.periscopedata.com/app/gitlab/825329/Editor-Extension-Category-MAU-Metrics)  Used frequently by Create : Code Review Group

* [Performance indicators internal handbook page](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/product/dev-section/)  The Create : Gitaly Group primarily uses the Performance Indicators Internal Handbook Page to guide decisions

* [Handbook page containing engineering analytics dashboards](https://about.gitlab.com/handbook/engineering/development/dev/create/engineering-managers/dashboards/)  Used by Create Stage Engineering Managers

**Important data documentation**

``` sql

SELECT * 
FROM table
WHERE field = stage_name
;
```

**Helpful video resources**

Must be logged into GitLab Unfiltered account

[Create Stage YouTube playlist](https://www.youtube.com/playlist?list=PL05JrBw4t0KrJEKqwt57ljmbkOuVwaR0d)

[Create Stage UX YouTube playlist](https://www.youtube.com/playlist?list=PL05JrBw4t0KrUvA91eFQedd6zrvH0_kGY)

**Product roadmap link**

[Link to product direction / vision](/handbook/engineering/development/dev/create/#vision)

Resource to understand the goals for this team

**Performance indicators**

[Link to performance indicators](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/product/dev-section/)

Resource to understand the Performance Indicators for the Dev Section - Page can be searched by Stage and Group

**Key handbook pages**

[Primary Create Stage handbook page](/handbook/engineering/development/dev/create/)

Contains helpful information about how Create operates and current team members

**Slack channels**

**#s_create** 

**#s_create_pm**

**Team members**

[Handbook page to find Create team members to collaborate with](/handbook/product/categories/#create-stage)

</details>

### Ops Section

#### Verify Stage
Verify provides teams with tools that help facilitate continuous integration. This includes but is not limited to pipelines and runners. 

<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Centralized SMAU / GMAU Dashboard](https://app.periscopedata.com/app/gitlab/758607/Centralized-SMAU-GMAU-Dashboard) This dashboard is a central place for all stages where their SMAU and GMAU metrics are housed for a high-level overview.

* [Ops Section Dashboard](https://app.periscopedata.com/app/gitlab/781120/Ops-Section-Dashboard) This is the central dashboard for all performance indicator metrics related to the Ops section. 

* [GitLab Runner SaaS Performance Indicator Metrics](https://app.periscopedata.com/app/gitlab/800667/GitLab-Runner-SaaS-performance-indicator-metrics)

* [Actions per Month Verify Stage Dashboard](https://app.periscopedata.com/app/gitlab/538594/Actions-Per-Month-Verify-Stage-Dashboard)

* [Error Budget Dashboard](https://app.periscopedata.com/app/gitlab/892433/Error-Budget-Dashboard---Stage-Verify)

**Important data documentation**

```sql
SELECT * 
FROM table
WHERE field = stage_name
;
```

**Helpful video resources**

[Tanuki Tech: Verify and Secure](https://youtu.be/TgRamhC3ujg)

This video showcases the product functionality of Verify and Secure and how to talk about those functionalities from a sales perspective.

[Verify Team Overview](https://youtu.be/9iF9zWAxdH0)

**Product roadmap link**

[Section Direction: Verify Stage](https://about.gitlab.com/direction/ops/#verify)
Resource to understand the long-term goals for the Verify team

**Performance indicators**

[Ops Section PI](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/product/ops-section/)
An internal handbook page that lists all performance indicators under the Operations section

**Key handbook pages**

[Verify Stage Product Page](https://about.gitlab.com/handbook/engineering/development/ops/verify/)

A central hub for all pages related to the Verify stage

**Slack channels**

**#s_verify**
Overall channel for Verify

**#g_pipeline-execution**
Slack channel for the Verify:Pipeline Execution product category. 

**#g_pipeline-authoring**
Slack channel for the Verify:Pipeline Authoring product category.

**#g_runner**
Slack channel for the Verify:Runner product category. 

**#g_pipeline-insights**
Slack channel for the Verify:Pipeline Insights product category.

**Team members**

[Handbook page to find Verify team members to collaborate with](/handbook/product/categories/#verify-stage)

</details>

#### Package Stage
The Package team works on the package and container registries, as well as the Dependency Proxy.

<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Package GitLab.com Stage Activity](https://app.periscopedata.com/app/gitlab/527857/Package-GitLab.com-Stage-Activity-Dashboard)

Primarily time series analyses for Package features on GitLab.com

* [Package: User Adoption and Growth](https://app.periscopedata.com/app/gitlab/805350/Package:-User-Adoption-and-Growth)

Primarily time series analyses including both SaaS and SM usage of Package features

* [Package customer adoption](https://app.periscopedata.com/app/gitlab/877343/Package-customer-adoption)

Customer specific data tables regarding specific Package feature usage

* [Package: Costs](https://app.periscopedata.com/app/gitlab/1011032/Package:-Costs)

Dashboard analyzing GCP costs associated with Package features. 

* [Package:-UI-Data](https://app.periscopedata.com/app/gitlab/1033908/Package:-UI-Data)

Dashboard measuring user interaction with the GitLab.com user interface.

**Important data documentation**

``` sql

SELECT * 
FROM table
;
```


**Helpful video resources**

[User Interviews YouTube Channel](https://www.youtube.com/playlist?list=PL05JrBw4t0KpxCv3B5S-6LFCpBB6NCnga)

General and feature specific user interviews for the Package team

[Demos and Speedruns](/handbook/engineering/development/ops/package/#demos--speedruns)

Package Handbook section with feature and roadmap demos

**Product roadmap link**

[Link to product roadmap](/handbook/engineering/development/ops/package/#roadmap)

Resource to understand the long-term goals for this team

**OKRs**

[Link to OKRs handbook page](/handbook/engineering/development/ops/package/#okrs)

Resource to understand the current OKRs for this team

**Key documentation**

[Main Package Team Handbook Page](/handbook/engineering/development/ops/package)

It can be helpful to search for specific topics on the Package team's main page

[GitLab Docs Package Page](https://docs.gitlab.com/ee/administration/packages/)

GitLab Docs are awesome!

**Slack channels**

**#s_package** 

**Team members**

[Handbook page to find Package team members to collaborate with](/handbook/product/categories/#package-stage)

[List of Package team members and their stable counterparts to contact if needed](/handbook/engineering/development/ops/package/#team-members)

</details>

#### Release Stage

GitLab's integrated CD solution allows users to ship code with zero-touch, be it on one or one thousand servers.

<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Release Stage Dashboard](https://app.periscopedata.com/app/gitlab/777879/Release-Stage-Dashboard) Primary point of reference for the Release Stage team. 


**Important data documentation**

``` sql

SELECT * 
FROM table
WHERE field = stage_name
;
```

**Helpful video resources**

[List of YouTube Playlists maintained by Release](https://about.gitlab.com/handbook/engineering/development/ops/release/#youtube-playlists)

**Product roadmap link**

[Product Direction - Release](https://about.gitlab.com/direction/release/#whats-next-and-why)
Resource to understand the long-term goals for this team

**Performance indicators**

[Link to performance indicators](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/product/ops-section/)

Resource to understand the Performance Indicators for the Ops Section - Page can be searched by Stage and Group

**Key handbook pages**

[Release Primary Handbook Page](https://about.gitlab.com/handbook/engineering/development/ops/release/)

**Slack channels**

**#s_release**


**Team members**

[Handbook page to find Create team members to collaborate with](/handbook/product/categories/#configure-stage)


</details>

#### Configure Stage

Enabling users to configure applications and infrastructure. Auto DevOps, Kubernetes Management and ChatOps.

<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Configure team business metrics](https://app.periscopedata.com/app/gitlab/511813/Configure-team-business-metrics) Central point of entry for the Configure Stage team to evaluate metrics.

* [Configure Stage Topic Board](https://app.periscopedata.com/app/gitlab/topic/Configure-Stage/ab515335d8494519ad4971740a62171a) Contains all of the most commonly used dashbaords by the Configure team.


**Important data documentation**

``` sql

SELECT * 
FROM table
WHERE field = stage_name
;
```

**Helpful video resources**

[GitLab <> Kubernetes Agent Overview](https://vimeo.com/677950027)

[AutoDevops Overview Demo](https://www.brighttalk.com/webcast/17523/524896) You'll need to register for brighttalk with your work email to access this resource.

**Product roadmap link**

[Product Direction - Configure](https://about.gitlab.com/direction/configure/#opportunities)
Resource to understand the long-term goals for this team

**Performance indicators**

[Link to performance indicators](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/product/ops-section/)
Resource to understand the Performance Indicators for the Ops Section - Page can be searched by Stage and Group

**Key handbook pages**

[Primary handbook page for Configure](https://about.gitlab.com/handbook/engineering/development/ops/configure/)

**Slack channels**

**#s_configure**

**Team members**

[Handbook page to find Create team members to collaborate with](/handbook/engineering/development/ops/configure/#team-members)


</details>

#### Monitor Stage

Helps reduce the severity and frequency of incidents. Incident management and error tracking.

<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Centralized SMAU/GMAU Dashboard](https://app.periscopedata.com/app/gitlab/758607/Centralized-SMAU-GMAU-Dashboard)

* [Error Budget Dashboard - Stage Monitor](https://app.periscopedata.com/app/gitlab/892457/Error-Budget-Dashboard---Stage-Monitor)


**Important data documentation**

``` sql

SELECT * 
FROM table
WHERE field = stage_name
;
```

**Helpful video resources**

Demos and overview videos for Monitor will be added here as they become available.

**Product roadmap link**

[Product Direction - Monitor](https://about.gitlab.com/direction/monitor/)
Resource to understand the long-term goals for this team

**Performance indicators**

[Link to performance indicators](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/product/ops-section/)

Resource to understand the Performance Indicators for the Ops Section - Page can be searched by Stage and Group

**Key handbook pages**

[Blog post on Incident Management](https://about.gitlab.com/blog/2021/11/30/gitlab-incident-management/)

**Slack channels**

**#s_monitor**

**Team members**

[Handbook page to find Monitor team members to collaborate with](/handbook/product/categories/#monitor-stage)

</details>

### Sec Section


#### Secure Stage

Static Application Security Testing (SAST), Dynamic Application Security Testing (DAST), Container Scanning, and Dependency Scanning 


<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Dynamic Analysis Metrics](https://app.periscopedata.com/app/gitlab/703762/WIP:-Dynamic-Analysis-metrics) Secure:Dynamic Analysis Group

Some seemingly duplicate charts in Dynamic Analysis Metrics are used by the team to compare totals from different data sets. 

* [Threat Management Metrics](https://app.periscopedata.com/app/gitlab/737412/Threat-Management-Metrics---Matt's-Playground) Govern:Threat Insights Group

* [Secure & Govern GMAU/SMAU Metrics](https://app.periscopedata.com/app/gitlab/707777/Secure-&-Protect-GMAU-SMAU-Metrics)
This dashboard shows various MAU metrics for Secure and Govern. 

* [Secure SCA - PI - Software Composition Analysis](https://app.periscopedata.com/app/gitlab/749790/Secure-SCA---PI---Software-Composition-Analysis---Schwartz) Secure:Composition Analysis Group



**Important data documentation**

``` sql

SELECT * 
FROM table
WHERE field = stage_name
;
```

**Helpful video resources**

[DevSecOps Overview](https://www.youtube.com/watch?v=XnYstHObqlA&t=15s) A great place to start for a high-level overview relating to Secure functionality.

**Product direction link**

[Secure product direction page - 1 year plan](https://about.gitlab.com/direction/secure/#1-year-plan)


**Performance indicators**

[Performance indicators linked in Secure handbook page](https://about.gitlab.com/handbook/engineering/development/sec/#performance-indicators)

**Key handbook pages**

[Secure stage primary handbook page](/handbook/engineering/development/sec/secure/)

**Slack channels**

**#s_secure**

**Team members**

[Product categories page section to find Secure team members to collaborate with](/handbook/product/categories/#secure-stage)

[Secure Handbook page section to find Secure engineering team members to collaborate with](/handbook/engineering/development/sec/secure/#team-members)


</details>


#### Govern Stage

Manage security vulnerabilities, policies, and compliance across your organization.

<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Security Policies Metrics](https://app.periscopedata.com/app/gitlab/694854/Container-Security-Metrics) Govern:Security Policies Group


**Important data documentation**

``` sql

SELECT * 
FROM table
WHERE field = stage_name
;
```

**Helpful video resources**

[Govern Stage YouTube Channel](https://www.youtube.com/playlist?list=PL05JrBw4t0Kq4CHpCTMv3OdquJXm6ggYr)

[Govern UX YouTube Channel](https://www.youtube.com/playlist?list=PL05JrBw4t0KrUL59mDTOdERpYEXGyMPVz)


**Product direction link**

[Govern product direction page - 1 Year Plan](https://about.gitlab.com/direction/govern/#1-year-plan)

**Performance indicators**

[Internal handbook performance indicators for the Secure section](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/product/sec-section/)

**Key handbook pages**

[Govern stage primary handbook page](https://about.gitlab.com/handbook/engineering/development/sec/govern/)

**Slack channels**

**#s_govern**

**Team members**

[Handbook page to find Govern team members to collaborate with](/handbook/product/categories/#govern-stage)

[Govern Handbook page section to find Govern engineering team members to collaborate with](https://about.gitlab.com/handbook/engineering/development/sec/govern/#sub-department-development-people-leaders)

</details>

### Enablement Section


#### Systems Stage (Distribution, Gitaly, Geo Groups)
Supports enterprise-grade operational experience of GitLab products from streamlined deployment and maintenance, disaster recovery, secure search and discoverability, to high availability, scalability, and performance. The Systems Stage includes Distribution, Gitaly and Geo Groups.


<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Enablement::Geo Metrics](https://app.periscopedata.com/app/gitlab/500159/Enablement::Geo-Metrics) Geo Group

* [Version Upgrade Rate](https://app.periscopedata.com/app/gitlab/406972/Version-Upgrade-Rate) Distribution Group

* [Enablement: Gitaly Dashboard](https://app.periscopedata.com/app/gitlab/728407/Enablement:-Gitaly-Dashboard) Gitaly Group

* [Centralized SMAU GMAU Dashboard](https://app.periscopedata.com/app/gitlab/758607/Centralized-SMAU-GMAU-Dashboard) General SMAU and GMAU metrics


**Important data documentation**

There are no Enablement metrics currently collected in our Postgres Replica data for Gitlab.com

The following tables can be used for Service Ping metric reporting. 

* common_mart.mart_ping_instance_metric_all_time - Use for all time timeframe metrics

* common_mart.mart_ping_instance_metric_7_day - Use for 7 day timeframe metrics

* common_mart.mart_ping_instance_metric_28_day - Use for 28 day timeframe metrics

* common_mart.mart_ping_instance_metric_monthly - Use for all, 7, 28 timeframe metrics pre filtered to the last ping of the month (does not include none or null timeframe metrics)

* workpace_product.wk_fct_ping_instance_metric_none - Use for metrics with a none timeframe

* workpace_product.wk_fct_ping_instance_metric_null - Use for metrics with a null timeframe

Use the [metrics dictionary](https://metrics.gitlab.com/) to determine the timeframe value for any service ping metric.


**Helpful video resources**

Enablement::Systems is a relatively new Stage. PDI will add helpful video overviews as they become available.

**Product roadmap link**

[Enablement Product Direction](https://about.gitlab.com/direction/enablement/)
Includes Stage and Group level details

**Performance indicators**

[Enablement Section PI handbook page](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/product/enablement-section/) 

**Key handbook pages**

[Overall Enablement Section Handbook page for Engineering](https://about.gitlab.com/handbook/engineering/development/enablement/)

**Slack channels**

**#s_enablement**

**#g_distribution**

**#g_geo**


**Team members**

[Handbook page to find Systems team members to collaborate with](/handbook/product/categories/#systems-stage)

OR

[All team members section of engineering page](https://about.gitlab.com/handbook/engineering/development/enablement/#all-team-members)

</details>

#### Data Stores Stage (Memory, Global Search, Database, Pods Groups)
Supports enterprise-grade operational experience of GitLab products from streamlined deployment and maintenance, disaster recovery, secure search and discoverability, to high availability, scalability, and performance. The Data Stores Stage includes Memory, Global Search, Database and Pods Groups.

<details markdown="1"><summary>Click to expand</summary>

**Top dashboards referenced by this team**

* [Enablement::Database - Performance Indicators](https://app.periscopedata.com/app/gitlab/754160/Enablement::Database---Performance-Indicators) Database Group

* [Enablement::Memory](https://app.periscopedata.com/app/gitlab/679200/Enablement::Memory) Memory Group

* [Global Search Self Managed Deep Dive](https://app.periscopedata.com/app/gitlab/1035187/Global-Search-Self-Managed-Deep-Dive) Global Search Group

* [gitlab.com performance per snowplow dashboard](https://app.periscopedata.com/app/gitlab/790506/gitlab.com-performance-per-snowplow-dashboard) Enablement Section overall - Primarily relates to Data Stores Group

* [Josh <> Mathieu: Enablement PPI](https://app.periscopedata.com/app/gitlab/794513/Josh-%3C%3E-Mathieu:-Enablement-PPI) - Enablement Section overall - Primarily relates to Data Stores Group

* [Active Instances](https://app.periscopedata.com/app/gitlab/441909/Active-Instances) - Database Group

* [Error Budget Dashboard - Stage Enablement](https://app.periscopedata.com/app/gitlab/892802/Error-Budget-Dashboard---Stage-Enablement) - Enablement Section overall

* [Infra PM Dashboard](https://app.periscopedata.com/app/gitlab/710777/Infra-PM-Dashboard) - Database Group

* [Enablement: Gitaly Dashboard](https://app.periscopedata.com/app/gitlab/728407/Enablement:-Gitaly-Dashboard) - Gitaly Group


**Important data documentation**

There are no Enablement metrics currently collected in our Postgres Replica data for Gitlab.com

The following tables can be used for Service Ping metric reporting. 

* common_mart.mart_ping_instance_metric_all_time - Use for all time timeframe metrics

* common_mart.mart_ping_instance_metric_7_day - Use for 7 day timeframe metrics

* common_mart.mart_ping_instance_metric_28_day - Use for 28 day timeframe metrics

* common_mart.mart_ping_instance_metric_monthly - Use for all time and 28 day timeframe metrics, pre filtered to the last ping of the month (does not include 7 day, none, or null timeframe metrics)

* workpace_product.wk_fct_ping_instance_metric_none - Use for metrics with a none timeframe

* workpace_product.wk_fct_ping_instance_metric_null - Use for metrics with a null timeframe

Use the [metrics dictionary](https://metrics.gitlab.com/) to determine the timeframe value for any service ping metric.

**Helpful video resources**

Enablement::Data Stores is a relatively new Stage. PDI will add helpful video overviews as they become available.


**Product roadmap link**

[Enablement Product Direction](https://about.gitlab.com/direction/enablement/)
Includes Stage and Group level details

**Performance indicators**

[Enablement Section PI handbook page](https://internal-handbook.gitlab.io/handbook/company/performance-indicators/product/enablement-section/) 

**Key handbook pages**

[Overall Enablement Section Handbook page for Engineering](https://about.gitlab.com/handbook/engineering/development/enablement/)

**Slack channels**

**#s_enablement**

**#g_memory**

**#g_global_search**

**#g_database**


**Team members**

[Handbook page to find Data Stores team members to collaborate with](/handbook/product/categories/#data-stores-stage)

OR

[All team members section of engineering page](https://about.gitlab.com/handbook/engineering/development/enablement/#all-team-members)

</details>

