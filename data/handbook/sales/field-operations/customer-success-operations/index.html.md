---
layout: handbook-page-toc
title: "Customer Success Operations"
description: "The Customer Success Operations team's handbook page. This covers our mission, strategies, responsibilities, and processes."
---
<link rel="stylesheet" type="text/css" href="/stylesheets/biztech.css" />

## On this page

{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

{::options parse_block_html="true" /}

## Mission

Customer Success Operations cross-functionally aligns GitLab for a superb customer experience through trust in data, clarity in effective processes, and predictability in customer and GitLab outcomes.

## Strategy

Develop and operationalize Customer strategies leveraging analytics and insights for key expansion and renewal initiatives, resulting in increased net ARR.

1. Operationalize Product Usage Data for customer value realization and outcomes
1. Enable customers through Digital Programs
1. Support customer renewal effectiveness through Renewal Operations
1. Increase Sales and CS effectiveness through systems and tools


## What we do

Customer Success Operations creates and updates existing processes for the Customer Success organization. CS Operations oversees:

- Systems implementation and maintenance
- Operational reporting
- Systems enablement
- Product analytics and renewal strategies
- Fiscal Year planning and strategy
- Operationalizing Customer Success Journeys

The CS Ops team also provides support for customer programs, renewals, and Gainsight.

<div class="flex-row" markdown="0" style="height:80px">
    <a href="/handbook/sales/field-operations/customer-success-operations/cs-ops-programs/" class="btn btn-purple-inv" style="width:30%;height:100%;margin:1px;display:flex;justify-content:center;align-items:center;">Customer Success Programs</a>
    <a href="/handbook/sales/field-operations/customer-success-operations/cs-ops-renewals/" class="btn btn-purple-inv" style="width:30%;height:100%;margin:1px;display:flex;justify-content:center;align-items:center;">Customer Success Renewals</a>
    <a href="/handbook/sales/field-operations/customer-success-operations/gainsight/" class="btn btn-purple-inv" style="width:30%;height:100%;margin:1px;display:flex;justify-content:center;align-items:center;">Gainsight Management<br> and Support</a>
</div>
<br>

## Who we work with

Customer Success Operations provides support, content, and data analysis for all Customer Success teams.

## CS Ops Request Process

![CS Ops Issue Flowchart](https://lucid.app/publicSegments/view/d1fded0a-7969-46d4-b300-0603d802e6e4/image.png "CS Ops Issue Flowchart")

## CS Ops Board, Groups, Projects, and Labels

### CS Operations Board

The CS Ops team uses issues and issue boards to track our projects and tasks. If you need help with a project, please open an issue and add the ~CSOps label anywhere within the GitLab repo.

CS Operations uses a [global issue board](https://gitlab.com/groups/gitlab-com/-/boards/3156857?label_name[]=CSOps) to capture and track issues in any group or sub-group in the repo.

See the [global issue board](https://gitlab.com/gitlab-com/sales-team/field-operations/customer-success-operations/-/boards/4341765?label_name[]=CS%20Ops%20Technical%20Writing) for CS Ops Technical Writing.

### Groups

- Use the `gitlab.com` group for epics that may include issues within and outside the Sales Team group.
- Use the GitLab Sales Team group for epics that may include issues within and outside the Field Operations group.

### Projects

Create issues in the [CS Operations project](https://gitlab.com/gitlab-com/sales-team/field-operations/customer-success-operations).

### Issue Weighting

- Weight = 1: 0-1 hours of work
- Weight = 3: 1-3 hours of work
- Weight = 5: 3-5 hours of work
- Weight = 7: 5-7 hours of work

Anything that takes longer than a day of work should be captured in an epic/multiple issues


### Labels

Labels to use when creating new issues or MRs for CS Ops:

**Team Specific or System Labels**
- **CSOps** - Use to track and manage all CS Operations-related issues and MRs.
- **CS Programs** - For the Digital Programs team to track and manage content requests, improvements, and other means of digital customer marketing.
- **CS Product Usage Reporting** - Issues related to Customer Success product usage data.
- **CS Analytics** - Used to track Customer Success Analytics issues.
- **CS RenewalOps** - Label to designate issues for the Renewal Ops team to improve our customer renewal process and experience.
- **CS Ops Technical Writing** - Assigned to the CS Ops technical writers for review or creation of copy.
- **Gainsight**- Label to designate the issue is related to Gainsight. 
- **Gainsight: Bug**- This label is used to track bugs exclusive to Gainsight.
- **Gainsight: Feature Request** - This label is used to track feature requests for our installation of Gainsight (not for Gainsight the product).

**Scoped Labels** - used for tracking SDLC progress
- **CSOps::Need_More_Info** - Requires additional information from the requester, or lacks information to complete the request.
- **CSOps::Ready_for_Assignment** - Ready to be assigned and prioritized by CS Ops.
- **CSOps::Awaiting Feedback**  - Used for peer review and when analysis is needed before closing the issue.
- **CSOps::In_Process** - Actively being worked on in the current week or milestone.
- **CSOps::Blocked** - Currently blocked by an internal or external prerequisite.
- **CSOps - Interrupt** - Issue that was submitted after the current milestone started and prioritized ahead of the original milestone scope.
- **CSOps::Triage**- Issue that is in the traige stage.
- **CSOps::Won’t Do** - Indicates that the issue is not going to be worked/completed, although scoping of solution might have already been concluded.

**Segment and Team Support Labels** - for tracking where the request(s) came from
- **CSOps - CSM- Ops** - Request opened by the CS Ops team that benefits the CSM team.
- **CSOps - CSM** - Request originating from the CSM team.
- **CSOps - PS** - Request originating from, or to benefit the PS team.
- **CSOps - SA** - Request originating from, or to benefit the SA team.
- **CSOps - Ops** - Request to benefit the CSOps team.
- **CSOps - PubSec** - Requests that are specific to the Pub Sec CSM Team.
- **CSOps - Strategic** - Requests that are specific to the Strategic CSM Team. 
- **CSOps - Scale** - Requests the are for the Scale Segment. 
- **CSOps - All Segments** - Request that cover all CS Segments. 
- **CSOps - Growth** -  Requests that are specific to the Growth CSM Team. 
- **CSOpsSlack-Questions** - Indicates that the request/issue came in via Slack (#gainsight-users Slack channel being the largest contributor to it)
- **CSOPs-Priority** - This is for initiative/issues tied to Top Priority Initiatives.

## Peer Review
The peer review process (currently for issues related to Gainsight) allows CS Ops team members to have another member of the team review their work.

The issue owner is responsible for making sure the issue is completed in timely manner, including communicating to the peer reviewer when the issue needs to be completed. The peer reviewer is responsible for completing the review in the timeframe given by the issue owner.

- Issues **MUST** be peer reviewed by the Gainsight Admin if it is a change, addition, or removal in a rule or data object (e.g. creating a new rule or connector job, removing fields from an object, combining multiple rules into one)
- For changes to reports or dashboards, strongly consider a peer review.

Feel free to ask for a peer review for other any updates if you feel it would be helpful to have a second opinion.

To start the peer review process:
1. Provide a Summary of the work you have completed in the **Resolution** section on the GitLab issue
2. Change the issue status to `CS Ops::Awaiting Feedback`
3. Tag the teammate completing the peer review and comment on the issue that it is ready for peer review
4. The issue owner will remain an assignee as they are ultimately responsible for the issue completion.
