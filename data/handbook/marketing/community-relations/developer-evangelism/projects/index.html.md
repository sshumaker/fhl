---
layout: handbook-page-toc
title: "Projects"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Introduction

We maintain our projects in the [gitlab-de group](https://gitlab.com/gitlab-de). This includes repositories for maintained [open source projects](/handbook/marketing/community-relations/developer-evangelism/oss-contributions/), workshops exercises, and more learning resources.

## Learning Collections

### Our Work Environments

* [Brendan's dotfiles](https://gitlab.com/brendan/dotfiles)
* [Michael's dotfiles](https://gitlab.com/dnsmichi/dotfiles) covered in [this blog post](https://about.gitlab.com/blog/2020/04/17/dotfiles-document-and-automate-your-macbook-setup/)

### log4j-resources

The [log4j-resources](https://gitlab.com/gitlab-de/log4j-resources) project provides a collection of resources to learn about, detect and mitigate the impact of the log4j vulnerability, more formally known as [CVE-2021-44228](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-44228).

Maintainers: [Developer Evangelism team](/handbook/marketing/community-relations/developer-evangelism/)

### o11y.love

[o11y.love](https://o11y.love/) is a collection of useful learning resources for observability. The [project](https://gitlab.com/everyonecancontribute/observability/o11y.love) is built using Markdown, MkDocs and GitLab Pages and organized in the [EveryoneCanContribute cafe](#everyonecancontribute-cafe) community. 

Maintainer: [Michael Friedrich](/company/team/#dnsmichi)

### Opentelemetry with GitLab Research

- Purpose: "Research OpenTelemetry with Tracing to help achieve CI/CD Observability in GitLab."
- Motivation: [Feature proposal for CI/Observability: Tracing with OpenTelemetry](https://gitlab.com/gitlab-org/gitlab/-/issues/338943)

The [project](https://gitlab.com/everyonecancontribute/observability/opentelemetry-gitlab-research) provides all notes, configuration, dev environments, research [changelog](https://gitlab.opentelemetry.love/changelog/), etc. and is deployed with GitLab Pages and MkDocs to [gitlab.opentelemetry.love/](https://gitlab.opentelemetry.love/). The subdomain is on purpose as long as the research continues; the main domain `opentelemetry.love` will be used by Michael for other projects. 

Maintainer: [Michael Friedrich](/company/team/#dnsmichi)

### opsindev.news Newsletter

[opsindev.news](https://opsindev.news) is a newsletter inspired by the problem of too many resources, spread around Slack channels and Twitter/LinkedIn feeds where the information can be overwhelming. The target audience is developers learning Ops and DevOps, as well as engineers facing day-2-ops challenges. The newsletter is based on the latest news, telling a story and diving into the latest technology. Tips and tools and CFPs for events are curated too.

The platform with Buttondown and GitLab pages is documented in the [Contributing guide](https://opsindev.news/contributing/). The newsletter is maintained in public in Michael's namespace: https://gitlab.com/dnsmichi/opsindev.news 

Maintainer: [Michael Friedrich](/company/team/#dnsmichi)

## Workshops

### DevOps and GitLab

#### DevOps with GitLab CI Course - Build Pipelines and Deploy to AWS

[GitLab Hero](/community/heroes/members/) [Valentin Despa](https://twitter.com/vdespa) created the 5h course in collaboration Michael Friedrich, who helped with the [course outline review](https://gitlab.com/everyonecancontribute/workshops/gitlab-ci-freecodecamp/-/merge_requests/1).

[![](https://img.youtube.com/vi/PGyhBwLyK2U/0.jpg)](https://www.youtube.com/watch?v=PGyhBwLyK2U "DevOps with GitLab CI Course - Build Pipelines and Deploy to AWS")

#### Efficient DevSecOps Pipelines in a Cloud Native World

The [slides](https://docs.google.com/presentation/d/12ifd_w7G492FHRaS9CXAXOGky20pEQuV-Qox8V4Rq8s/edit) provide a 10+ hours workshop created by Michael Friedrich for the Open Source Automation Days 2021. The exercises in the slides refer to [a workshop project](https://gitlab.com/gitlab-de/workshops/ci-cd-pipeline-efficiency-workshop) which also includes the solutions.

The following topics will be practiced:

- Introduction: CI/CD meets Dev, Sec and Ops
- CI/CD: Terminology and first steps
- Analyse & Identify
  - Learn using the [GitLab CI Pipeline Exporter](https://github.com/mvisonneau/gitlab-ci-pipelines-exporter/tree/main/examples/quickstart) to monitor the exercise project throughout the workshop.
- Efficiency actions
  - Config Efficiency: CI/CD Variables in variables, job templates (YAML anchors, extends), includes (local, remote), rules and conditions (if, dynamic variables, conditional includes), `!reference` tags (script, rules), maintain own CI/CD templates (include templates, override config values), parent-child pipelines, multi project pipelines, better error messages to fix failures fast 
  - Resource Use Efficiency: Identification, max pipeline duration analysis, fail fast with stages grouping, fail fast with async needs, analyse blocking stages pipeline (solution with needs), matrix builds for parallel execution (pratice: combine matrix and `extends`, combine matrix and `!reference`), `extends` merge strategies (with and without `!reference`)
  - CI/CD Infrastructure Efficiency: Optimization ideas, custom build images, optimize builds with C++ as example, GitLab runner resource analysis (sharing, tags, external dependencies, Kubernetes), local runner exercise, resource groups, storage usage analysis, caching (Python dependency exercise, including `when:always` on failed jobs) 
  - Auto-scaling: Overview, AWS auto-scaling with GitLab Runner with Terraform, insights into [Spot Runners on AWS Graviton](https://about.gitlab.com/blog/2021/08/17/100-runners-in-less-than-10mins-and-less-than-10-clicks/)
- Group discussion
  - Deployment Strategies: IaC, GitOps, Terraform, Kubernetes, registries
  - Security: Secrets in CI/CD variables, Hashicorp Vault, secrets scanning, vulnerability scanning
  - Observability: CI/CD Runner monitoring, SLOs, quality gates, CI/CD Tracing
  - More efficiency ideas: Auto DevOps, Fast vs Resources, Conclusion and tips

<figure class="video_container">
<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vQCF72s_IIogKurtLhEZ3Pe3SrkcRL1KYIhScYwhwPlFDJTGYLK_sZGnG4gAfy0jiiQnITuxSGPDB48/embed?start=false&loop=false&delayms=3000" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
</figure>



### Template: Basics and CI/CD with the Go Tanuki

The [slides](https://docs.google.com/presentation/d/1bj8FqU5I-Og-Yf9rDbp0qRjV4AXQo8K-rfOXkSUClW4/edit?usp=sharing) provide the step-by-step instructions as exercises for the [GitLab CI/CD Go Tanuki workshop](https://gitlab.com/gitlab-de/workshops/gitlab-cicd-go-tanuki-workshop):

- First Steps with GitLab
- CI/CD: Getting Started
- CI/CD: Go Project and Tests
- Security with GitLab
- Deliver and Deploy
- What's next
- Exercises for async practice
- Efficiency practice

#### Recent Recordings

[![](https://img.youtube.com/vi/id9klDUrGN8/0.jpg)](https://www.youtube.com/watch?v=id9klDUrGN8 "TalentQL Pipeline workshop in October 2021")
[![](https://img.youtube.com/vi/kTNfi5z6Uvk/0.jpg)](https://www.youtube.com/watch?v=kTNfi5z6Uvk "1. Swiss Meetup 2021 in January")

Recordings of past workshops and other videos from the Developer Evangelism team can be found on our [team playlist](https://www.youtube.com/playlist?list=PL05JrBw4t0Kq-bYO9jCJaN45BBpzWSLAQ) on GitLab Unfiltered. 

### Past Meetup Workshops

Meetup workshops are available in the [workshops group](https://gitlab.com/gitlab-de/workshops) in the GitLab Developer Evangelism group. Note that the content, exercises and source code evolved over time :)

#### Basics and CI/CD

- [TalentQL Pipeline workshop in October 2021](https://gitlab.com/gitlab-de/workshops/go-tanuki-cicd-workshop-talentql-pipeline-program)
- [1. Swiss Meetup 2021 January](https://gitlab.com/gitlab-de/workshops/swiss-meetup-2021-jan)
- [Morehouse College CI CD Lecture](https://gitlab.com/gitlab-de/workshops/morehouse-college-lecture-cicd)
- [CI Community Day 2020](https://gitlab.com/gitlab-de/workshops/ci-community-day-2020)
- [KDE Akademy Workshop 2020](https://gitlab.com/gitlab-de/workshops/kde-akademy-workshop-2020)
- [LA / SoCal / Orange County Meetup 2020](https://gitlab.com/gitlab-de/workshops/meetup-2020-cw41)
- [Collision from Home GitLab CI workshop](https://gitlab.com/gitlab-de/workshops/collision-from-home-2020)
- [Linuxing London Meetup - GitLab Introduction](https://gitlab.com/gitlab-de/workshops/meetup-2020-cw17)
- [First virtual GitLab meetup - intro to CI](https://gitlab.com/gitlab-de/workshops/meetup-2020-cw13)

German language:

- [German CI/CD Workshop 2021](https://gitlab.com/gitlab-de/workshops/german-cicd-workshop-2021-jan)

#### Monitoring and Security

- [Identify, analyze, action! Deep monitoring with CI](https://gitlab.com/gitlab-de/workshops/ci-monitoring-webcast-2020)
- [GitLab CI Security Webcast](https://gitlab.com/gitlab-de/workshops/ci-security-webcast-2020)


### Thought Leadership: Observability

#### Kubernetes Observability workshop for Kube Simplify

Michael Friedrich provides a 3.5 hours live workshop on Kubernetes Observability for the [Kube Simplify workshop series](https://kubesimplify.github.io/live-workshops/) as a free learning resource. After an introduction, the workshop starts with an overview of monitoring, metrics with Prometheus, and how to build and use dashboards in Kubernetes. Alerts, incidents and SLOs are practiced by example, building the bridge into more Observability data with tracing, logs and more event types. Chaos engineering is practiced with Chaos Mesh to trigger alerts when DNS errors force an app to leak memory. This allows users to practice the [KubeCon EU 2022 demo](https://youtu.be/BkREMg8adaI) themselves. Scaling, long term storage, security workflows as well as new innovative ideas with OpenTelemetry and eBPF are discussed too. The workshop includes exercises and solutions ready for production environments afterwards. 

Resources:

- [Slides with exercises](https://docs.google.com/presentation/d/1uuYIPwQjckNiPPJQcN8tauZ8KSIdHASbyoAxJ0fc6uQ/edit?usp=sharing)
- [Project with solutions](https://gitlab.com/everyonecancontribute/workshops/kube-simplify/k8s-o11y-2022)

Recording:

[![Kube Simplify: Kubernetes Observability workshop](https://img.youtube.com/vi/sMEEVbZ4NFM/0.jpg)](https://www.youtube.com/watch?v=sMEEVbZ4NFM)


#### Practical Kubernetes Monitoring with Prometheus

The [slides](https://docs.google.com/presentation/d/17XVCbiC4PZYvpreZINmhNltmT-DDCo3LjoaPgqpsxVo/edit) provide a 4+ hours workshop, more details are available [on Michael Friedrich's personal blog](https://dnsmichi.at/2021/09/14/monitoring-kubernetes-with-prometheus-and-grafana-free-workshop/). The following topics will be practiced:

- Monitoring, quo vadis puts the traditional monitoring in contrast to microservices.
- Prometheus and Grafana shares the basic knowledge on Prometheus, PromQL, Service Discovery and terminology required to understand.
- Kubernetes dives into understanding what to monitor, and how.
- Prometheus Operator dives into the concept of the package, and kube-prometheus installing a full stack. You'll dive into the UI of Prometheus, Grafana and the Alert Manager.
- K8s monitoring with Prometheus walks you through the - amazing - default Grafana dashboards, instructs you to deploy a Go demo app with the CRD ServiceMonitor, Container Metrics and kube-state-metrics exercises to practice PromQL queries.
- Advanced Monitoring practices with a Python app and own metrics, deployed to the GitLab container registry and to Kubernetes to query with PromQL in Grafana dashboards. Storage with Thanos/Cortex, Service Discovery is touched as well.
- Alerts and Escalations dives into the Alert Manager and rules, mapped into the PrometheusRule CRD.
- SLA, SLO, SLI keeps you busy with learning about Service Level Objectives for your production environment, providing thoughts on CI/CD quality gates with Keptn - and the OpenSLO spec, Pyrra and Sloth.
- Observability moves from Monitoring to metrics, logs, traces and beyond.
- Secure Monitoring discusses TLS, secret management, Infrastructure as code workflows, Container security and RBAC & policies.
- Ideas on more monitoring with Prometheus exporters, podtato-head, Chaos Engineering, etc.

A shorter version of the workshop [as a talk](https://docs.google.com/presentation/d/1EEBJFgeThlVEeC_E3tOYGicU2X0S9vPGsba49EQSNwk/edit) was provided by Michael Friedrich at PromCon NA 2021, a zero day event at KubeCon NA.

[![](https://img.youtube.com/vi/CyQNYT1ZQQ8/0.jpg)](https://www.youtube.com/watch?v=CyQNYT1ZQQ8 "PromCon NA: Practical Kubernetes Monitoring with Prometheus")





## OSS Projects

The Developer Evangelism team maintains [OSS projects](/handbook/marketing/community-relations/developer-evangelism/oss-contributions/) as part of community activities. 

### CodeChallenge.dev

Maintainer: [Abubakar Siddiq Ango](/company/team/#abuango)

`CodeChallenge.dev` is an app that you can use to create challenges that are tied to actions in GitLab.  For example, you can create a challenge that teaches folks how to make merge requests, add issues, or use other GitLab features.  Currently in the beta release, the Code Challenge software was first used at KubeCon EU 2022.

Homepage: [CodeChallenge.dev](https://codechallenge.dev)

Documentation: [docs.codechallenge.dev](https://docs.codechallenge.dev)

Project: [codechallenge](https://gitlab.com/gitlab-de/codechallenge)

<figure class="video_container">
    <iframe src="https://www.youtube.com/embed/BNEQMNtrlSM" frameborder="0" allowfullscreen="true"> </iframe>
</figure>


### Evangelist Dashboards

Maintainer: [Abubakar Siddiq Ango](/company/team/#abuango)

The dashboard is the SSoT to collect all metrics for the Developer Evangelism, and Education Evangelism teams. This includes Twitter, CFPs, YouTube/Google Analytics, etc. Next to the dashboard component, the data component ensures to collect all data from different APIs and sources, and [gets deployed to GitLab pages](https://gitlab-de.gitlab.io/dashboards/).

Project: [Dashboards](https://gitlab.com/gitlab-de/dashboards)

### Developer Evangelism Bot

Maintainer: [Abubakar Siddiq Ango](/company/team/#abuango)

This bot aims to automate the team tasks such as:

* Create [release evangelism](/handbook/marketing/community-relations/developer-evangelism/social-media/#release-evangelism) issues for team members.
* Triage issues following the [Developer Evangelism workflows](/handbook/marketing/community-relations/developer-evangelism/workflow/).
* Generate an issue letter (created, closed, open CFPs) on every Monday.

Project: [DE Bot](https://gitlab.com/gitlab-com/marketing/corporate_marketing/developer-evangelism/code/de-bot)

### Developer Evangelism Dashboard

Maintainer: [Abubakar Siddiq Ango](/company/team/#abuango)

This [custom dashboard](https://gitlab-com.gitlab.io/marketing/corporate_marketing/developer-evangelism/code/de-dashboard/) is built using [GitLab pages](https://about.gitlab.com/stages-devops-lifecycle/pages/) and presents an overview of Developer Evangelism issues. The requests are synced in a specified interval.

Project: [DE Dashboard](https://gitlab.com/gitlab-com/marketing/corporate_marketing/technical-evangelism/code/de-dashboard)

### Youtube2Sheets

Maintainer: [Abubakar Siddiq Ango](/company/team/#abuango)

This project is used internally at GitLab to retrieve the list of videos from specified playlists on Youtube onto a specified Google Sheet. Pipeline is scheduled to run at midnight and noon UTC.

Project: [Youtube2Sheets](https://gitlab.com/gitlab-com/marketing/corporate_marketing/developer-evangelism/code/youtube2sheets)


### Events Project

Maintainer: [Abubakar Siddiq Ango](/company/team/#abuango)

The Developer Evangelism Team at GitLab tracks events happening across the industry for attendance, speaking engagements, or just to keep them on the radar. This is also a major need across the industry. The Events project aims to provide an open and collaborative place where members of the wider GitLab community can add and track events happening in the industry.

Project: [DE Events Project](https://gitlab.com/gitlab-de/events)


## EveryoneCanContribute cafe

Maintainer: [Michael Friedrich](/company/team/#dnsmichi)

[everyonecancontribute.com](https://everyonecancontribute.com) serves as the main website for a community formed around tech coffee chats called `#EveryoneCanContribute cafe` (active) and `#EveryoneCanContribute Kaeffchen` (retired).

The coffee chats are organized as [meetup.com group events](https://www.meetup.com/everyonecancontribute-cafe/) and are open for topic or theme suggestions from everyone. 

* Try out newly announced projects together.
* Do pair programming/debugging sessions.
* Start discussions and share ideas on the latest technology.

The sessions are hosted by Michael Friedrich. Developer Evangelism team members are assigned as alternative hosts in Zoom. The meetups are hosted in Zoom with a waiting room as default, the Zoom URL is hidden in the meetup group event. team members can access the URL in the [Developer Evangelism team calendar](/handbook/marketing/community-relations/developer-evangelism/). For joining the group, users need a profile picture and provide their name for joining an event. This is to protect against Zoom bombing and otherwise harmful intentions. 

Next to Zoom, everyone can hangout with text or audio in [Discord](https://everyonecancontribute.com/page/handbook/#discord).

The website's [About page](https://everyonecancontribute.com//page/about/) covers more details including the exact date and time.

Insights:

* The website is built using [GitLab pages](https://about.gitlab.com/stages-devops-lifecycle/pages/).
* Organization happens in the GitLab group [everyonecancontribute](https://gitlab.com/groups/everyonecancontribute/-/issues). This group has applied for an Ultimate license for OSS projects.
* [#everyonecancontribute cafe (English)](https://www.youtube.com/playlist?list=PL05JrBw4t0Kp1Gni9SyudMmXmBJIp7rIc) YouTube playlist.
* [#everyonecancontribute Kaeffchen (German)](https://www.youtube.com/playlist?list=PL05JrBw4t0Ko8J8V5V794CXZUZ-DLxccI)YouTube playlist.

[everyonecancontribute.dev](https://everyonecancontribute.dev) hosts a demo page with funny animations featuring the Tanuki, Clippy, and more. It is deployed in a container environment and provides a Prometheus node exporter for monitoring demos and talks. Michael created the website for the job application presentation panel at GitLab.

### Metrics and Insights

In order to track the sessions, [create a monthly issue report](https://gitlab.com/gitlab-com/marketing/corporate_marketing/corporate-marketing/-/issues/new?issuable_template=everyonecancontribute-cafe-insights) with linking the blog post, recording, social shares etc. 

### everyonecancontribute cafe groups

- [Kubernetes](https://gitlab.com/everyonecancontribute/kubernetes) with hands-on workshop series.
- [Keptn, GitLab, Prometheus](https://gitlab.com/everyonecancontribute/keptn) to collaborate on a deeper integration.
- [5minprod.app](https://gitlab.com/everyonecancontribute/5-min-prod-app) to drive the [5 minute production app](https://gitlab.com/gitlab-org/5-minute-production-app/deploy-template) with community resources.




