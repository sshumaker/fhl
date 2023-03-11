---
layout: handbook-page-toc
title: "Research insights"
description: "Research insights are the collective findings and learnings that come from a research study."
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

#### What is an insight? 
When we conduct research studies, we have a set of [goals and objectives](/handbook/product/ux/ux-research/defining-goals-objectives-and-hypotheses/) that guide us as we investigate research questions. Whether we're evaluating the usability of a feature, conducting exploratory interviews, or gathering quantitative data, the research study will likely result in a list of observations, patterns, and behaviors related to a user's experience. The raw data from the study are the research findings.

A list of findings, alone, is often not enough to fully communicate how users conceptualize a topic or why they experienced a certain struggle. Through [analysis and synthesis](/handbook/product/ux/ux-research/defining-goals-objectives-and-hypotheses/) of the data gathered in a research study, we are able to distill *insights* that connect the dots between related concerns and provide an additional layer of understanding. These synthesized research findings evolve into a cohesive collection of insights that enables stakeholders to make informed decisions. We support each insight with evidence that can be referenced during discussions, typically in the form of video clips, interview quotes, or statistical data.

At GitLab, we measure the impact of our research by:  

* Distinguishing an insight as "actionable" or "informative"
* Making sure each actionable insight has a clear recommendation or action associated with it
* Tracking the completion of actionable insights

There are two types of insights: **Actionable** and **Informative**.

  - Actionable insights are findings that require an action to be taken to resolve them. These can include UI changes, feature additions, and even conducting additional research.  All of these insights require the person conducting the research to create a GitLab issue that documents the actionable insight along with a proposed path for a solution.
  - Informative insights are findings that provide additional insights into topics, but for which no action needs to be taken as there is nothing to resolve. Informative insights are created only in Dovetail.

#### Informative insights
Informative insights help us learn about something or someone and don’t result in immediate action. Instead, these insights help build knowledge about our users, industries, competitors, and so on. For example:

> * Most developers who took part in the survey were first introduced to GitLab while they were in school.
> * Developers use about three other applications in addition to GitLab as part of their jobs.

When documenting informative insights, no special actions or processes need to be followed. These simply get documented into Dovetail, per the [standard process](/handbook/product/ux/dovetail/).

#### Actionable insights
Actionable insights **always have a follow-up action** that needs to take place as a result of the research observation or data, and a clear recommendation or action associated with it. An actionable insight both defines the insight and clearly calls out the next step. Here are two different examples:

> * Users weren't able to submit a merge request in the proposed design because they couldn't find the “Submit” button. They expected it to be located at the top of the page. Action: Iterate on the design to relocate the 'Submit' button to the top of the page and retest (link to Issue # XYZ).

> * IT Admins want a way to view all of their teams' activity over time, in 15 min increments. IT Admins are being asked to report on this information as part of a new company policy. Action: Explore the feasibility of such a request (link to Issue # ABC).

When creating an actionable insight issue to propose a change to a feature or product area under use, be cognizant of the wider impact of the changes on the top JTBDs associated with that area. If the data backing the insight does not provide enough confidence in the highlighted problem, take [additional measures to validate it](/handbook/product/ux/jobs-to-be-done/#quick-methods-to-increase-confidence).  

### How to document actionable insights
Actionable insights need to be handled differently than informative insights. Actionable insights are tracked over time and will include follow-up, so document actionable insights in Dovetail and in GitLab as unique Issues. 

When you document an actionable insight, its three main components are:

1. The insight itself: often the problem, finding, or observation.
1. The “why”: supporting evidence that supports the insight. Often, it’s describing why the problem is happening, or more details behind the finding or observation. 
1. The action: the next step or action that needs to take place as a result of the research. The action should be clearly defined, achievable, and directly tied back to the insight.  

Tips for writing an actionable insight:
* Avoid using words like: consider, possibly, maybe, suggest, etc. People can interpret these actions as optional. 
* Instead, use directive terminology, such as: conduct, explore, redesign, etc. These words contribute to a clear action that needs to be taken as a next step.

To document actionable insights:

* **Step 1:** In Dovetail, preface the actionable insight's title with 'ACTIONABLE:' and clearly describe the next action that needs to be taken.
* **Step 2:** Create a unique issue in [GitLab.com](https://gitlab.com/gitlab-org/gitlab/-/issues/new) using the appropriate _Actionable Insight_ issue template:
     * **Actionable Insight - Exploration needed** -  This is an actionable research insight derived from a UX research study. To address this insight, further exploration is required. That might be in the form of follow-up research, design explorations, etc. This issue template includes the `~"Actionable Insight::Exploration needed"` scoped label.
     * **Actionable Insight - Product change** -  This is an actionable research insight derived from a UX research study. To address this insight, a change to the product experience is required. This issue template includes the `~"Actionable Insight::Product change"` scoped label.  _Note that the `~"SUS::Impacting"` label and a [severity label](/handbook/engineering/quality/issue-triage/#severity) are both required for actionable insights that require product changes._
     
   Both templates use a corresponding scoped label (above) to keep track of the progress being made regarding next step(s). To streamline this process, add a link to the Dovetail insight in the GitLab issue, rather than typing out all the details again. (If you want to include details, you certainly can.)
* **Step 3:** Add the appropriate `Group` (such as `~"group::source code"`) label to the issue.  This is done to identify and track actionable insights at the group level.
* **Step 4:** Using the related issue feature, link these Actionable Insight issues back to the original Research Issue in the GitLab UX Research project.

#### Do I need to create a new actionable insight issue when the insight is already documented in another issue? 
If the insight is already documented within an issue, you can add an `~"Actionable Insight::Product change"` or `~"Actionable Insight::Exploration needed"` label to avoid redundant documentation. However, it is important to ensure the existing issue accurately addresses 1) the insight and 2) what needs to be done. When one or both aspects are lacking in detail, you will need to update the existing issue **before** adding a label.

#### Who creates and manages actionable insights?
Actionable insights are created and managed by the person closest to the research, which is typically the Product Manager, Product Designer, or UX Researcher.
However, it’s ultimately up to the team to decide who manages actionable insights.

#### How to manage actionable insights

All discussions and decisions made about the actionable insight must be documented within the issue, because these issues are tracked as performance indicators. As we track actionable insights over time, it’s important to understand what kinds of decisions we’re making based on user research.

When closing an actionable insight issue, *it’s important to document why it was closed and whether the original action was acted upon.*

In some cases, no action will be taken for a number of reasons, such as low priority, too large of an effort, not technically feasible, and so on. Regardless of the reason, document the decisions in the issue when closing it.

#### To what kinds of validation research do actionable insights apply?

Both Problem Validation and Solution Validation need to follow the actionable insights documentation process if actionable insights are discovered. For example:

* **Problem Validation:** If there are insights that result in additional research, a newly identified target for next steps, or an identified problem to address, those are actionable insights.
* **Solution Validation:** If there are insights that uncover a usability issue, a pain point users may experience, or a design issue, those are actionable insights.

The above examples have one thing in common regardless of the kind of research: the insight is actionable, and therefore, must be documented as such.

Additionally, UX Scorecard testing can yield actionable insights. Since UX Scorecard testing is an expert review and/or heuristic evaluation, creating Dovetail insights may not be applicable. Instead, be sure to document the details in the GitLab issue using the actionable insight template in [GitLab.com](https://gitlab.com/gitlab-org/gitlab/-/issues/new).

We label issues containing insights identified through customer calls differently than other insights, because they don't directly relate to UX research efforts or tracking. For issues that contain insights derived from customer calls (or other customer support channels), please use the `~"Customer feedback"` label.

### Why we track actionable insights

Actionable insights are tracked at GitLab for:

* **Accountability:** If there’s something that needs to be done as a result of conducting research, it should be done. This process helps prevent those actionable insights from getting lost, dismissed, or taking too long to be acted upon.
* **Measuring research impact:** Presently, it’s difficult to accurately measure the impact of a research project on the product. Tracking actionable insights allows us to refer back to a particular research project, see what actions were identified as a result of the research findings, and determine what action was taken within the product since those actions were identified.

The following data is presently being tracked:

* **Number of newly opened and closed actionable insights issues, by quarter**
   * How many new actionable insight issues were created, per quarter
   * How many actionable insight issues were closed, per quarter - and why they were closed
* **Average number of days it takes for an actionable insight issue to close to completion**
   * Important to understand how long it's taking to address actionable insights within the product
* **Breakdown of all actionable insight issues, to date**
   * Provides us with an understanding of how many total actionable insights there are, broken down by open and closed statuses

The data for the above can be viewed for each actionable insight scoped label:
* [Actionable insight::Product change](https://app.periscopedata.com/app/gitlab/1076087/Actionable-Insights::Product-Change)
* [Actionable insight::Exploration needed](https://app.periscopedata.com/app/gitlab/1076091/Actionable-Insights::Exploration-Needed)

Over time, once there's enough data, we might be able to slice this data at the stage/group level to help us understand what is (or isn't) working well. Based on what we learn, we’ll iterate on the approach.

Future data tracking considerations for actionable insights:

* **Number of total actionable insights currently open, no activity within the issue** (>6 month of no activity)
   * Total number of actionable insights that have not seen activity in at least a month.  These actionable insights will be followed up to understand why there hasn’t been activity.
* **Number of total of actionable insights currently open, activity within the issue** (activity <=6 months ago)
   * Total number of actionable insights that have seen activity within the past month.  It’s implied that these are actively being addressed in some way and not discarded.

#### How we document actionable insights as closed
Regardless of the type of actionable insight, we groom each closed actionable insight issue and assign the proper `closed::` scoped label to them.  Presently, this is a manual process done every other week by the UX Research Leadership team via a Slack bot notification. UX Research leaders start by understanding why the actionable insight issue was closed, then simply adding the correct `closed::` scoped label to it. An existing Sisense query then picks ups the issue for reporting purposes.

#### Creating useful insights
It's important to remember that insights often need context, since people may read them in isolation and misinterpret them. As you work on reporting on your study, it's important to keep the audience in mind and think about what you'd like them to learn from the study.

For example, you may find it useful to document all insights (big or small) from studies conducted on the GitLab interface to provide an explanation for why the interface has changed over time. This creates a record of why previous design decisions were not ideal, which can be helpful for discussions with newer team members. On the other hand, for design evaluations or tests with prototypes, it may be more relevant to focus on documenting the insights that answer the overarching research questions, since these studies often result in additional design iterations before implementation.

In either case, adding a brief "context" section at the top of the project description and providing a link to the relevant design artifact can help the reader better understand the background of the study.

#### Leveraging Dovetail insights
Searching through Dovetail is a great way to get acquainted with GitLab users and learn about studies that have already been conducted. You can search and filter through insights, highlights, tags, and charts to find the research that is relevant to any stage, feature, and type of research.

Another approach is to look through the [GitLab workspace homepage](https://dovetailapp.com/home/) in Dovetail if you'd like to see a higher-level overview of research being conducted across the stages (internal access only).

Whether you're looking to better understand a user persona, learn about use cases for features, gather context for solving a problem, or plan a future research study, Dovetail has something for you.

#### Collating insights from multiple studies
Also known as [desk research or secondary research](https://www.nngroup.com/articles/secondary-research-in-ux/). Sometimes it can be helpful to summarize and collate existing research to have a broader picture of users outside of a specific study. Insights from past studies can serve as a foundation for future studies and provide a high level overview of user behaviors and mental models. 

To document insights from multiples studies, [tag themes and create insights](/handbook/product/ux/dovetail/) within individual Dovetail projects. Create a separate Dovetail story or project to summarize findings from multiple studies. Create an issue in GitLab which outlines the collated research project. Within that issue, add relevant Dovetail links and related issues.
