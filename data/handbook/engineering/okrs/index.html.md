---
layout: handbook-page-toc
title: Engineering OKRs
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

Here is the [standard, company-wide process for OKRs](/company/okrs/). Engineering has some small deviations from (and extensions to) this process.

## OKRs that require Product to schedule work

We sometimes have Engineering OKRs that require assistance from Product to ensure the issues are scheduled in that quarter. An example would be work to burn down our [SUS backlog](https://about.gitlab.com/handbook/product/ux/performance-indicators/system-usability-scale/). As our quarters use calendar months, and our product development means we [release every month on the 22nd](/handbook/engineering/releases/#timelines), there is a disconnect that means we should start planning earlier. While the preference is for a portion of the issues to be in [validation phase 3](/handbook/product-development-flow/#validation-phase-3-design) and ready to be scheduled for the first milestone of a quarter (which starts just before the fiscal quarter), some items may roll over to the first milestone in the following quarter. OKR scoring takes this timeline disconnect into account. See the [Product OKR process](/handbook/product/product-okrs/) for more information.

As a result, Engineering will begin communicating with Product **6 weeks before the start of the quarter** regarding any possible upcoming OKRs that need scheduling assistance from PMs. The goal is at **4 weeks before the start of the quarter** Engineering will confirm alignment with Product on shared OKRs. See the [Product OKR timeline](/handbook/product/product-okrs/) for more details. There is no set number for joint OKRs, and should not be a large proportion of Engineering OKRs in any quarter.

As this is earlier than the typical company timeline for OKRs, the exact timeline may shift depending on the [CEO OKR timeline](/company/okrs/#okr-process-at-gitlab), and drafting should begin based on top business need including [top initiatives](/company/top-cross-functional-initiatives/), [3 year strategy](/company/strategy/#three-year-strategy), and especially [FY direction](/direction/).

## OKR Kickoff

This process should begin no later than two weeks before the end of the preceding quarter. And kickoff should happen on or before the first day of the new quarter.

If you need guidance on writing OKRs, please refer to the [fundamentals of OKR at GitLab](/company/okrs/#fundamentals-of-impactful-okrs), which includes OKR examples and additional resources.

1. OKR owners should author OKRs.
1. Get approval **prior to the first day of the quarter** from your manager.
    - Use 1:1 with CTO to review
    - For everyone else: Ask you manager to do an async review of your OKRs, or discuss in a 1:1.
1. Communicate dependencies to other divisions, departments, or teams. Encourage them to take on corollary OKRs.

## Scoring guidelines

We will use the following guidelines for consistency.

1. Progress percentage is automatically updated based on child objectives or KRs.
1. For manually updated percentages, ensure to include an explanation of how the percentage is calculated in the OKR description.
  * The calculation can be simple "% of goal, 30 S2 bugs from <link>".
  * Consider breaking down project or task KRs. For example, "10% gathering data, 20% analyzing data, 20% summary of data, 20% write proposal, 10% gather feedback, 20% decide and open epic with issues with work required".
1. For scoring KRs that apply to a **rate** (for instance, [MR rate](../metrics/#merge-request-rate)), we score them as follows:
  * Take the initial rate before the quarter. For example, this is 10.
  * Take the target rate at the end of the quarter. In this example, it is 17.
  * Subtract initial rate and target rate to determine the target increase: 17 - 10 = 7.
  * Each month, take that month's rate and calculate our progress towards the target independently. For example:
      * Month 1: 12. The score is (12 - 10) / 7 = 2 / 7.
      * Month 2: 13. The score is (13 - 10) / 7 = 3 / 7.
      * Month 3: 15. The score is (15 - 10) / 7 = 5 / 7.
  * Take the score for the month, divide it by three, and add it to the total score. In the above example:
      * Month 1: 2 / 7 / 3 ~= 9.5%.
      * Month 2: 3 / 7 / 3 ~= 14%. Added to the previous month, the score is now 23.5%.
      * Month 3: 5 / 7 / 3 ~= 24%. Added to the previous months, the final score is 47.5%.

## Entering OKRs

For instructions, please refer to the ["How to use GitLab for OKRs" section on the OKR page](/company/okrs/#how-to-use-gitlab-for-okrs).

Some specific guidance:

1. [Decide on an objective or key result](#deciding-between-an-objective-and-key-result-in-gitlab).
1. Title: Avoid adding a "FYXX-QX" prefix as it's indicated by the milestone.
1. Description:
    1. If a GitLab issue or epic exists, make sure to include a link to it.
    1. Mention [how the OKR is scored](#scoring-guidelines).
1. All other fields including assignee and labels: follow the [company guidance](/company/okrs/#how-to-use-gitlab-for-okrs).

### Deciding between an objective and key result in GitLab

Create a new or "child" objective if the OKR will be broken down further and will be scored based on its children (see next section). If there will be no children, create a key result.

If you're unsure, we recommend creating a child objective.
If an objective or key result needs to be changed to the other type, you will need to re-create it and delete the "old" work item.

### CTO OKR alignment and scoring

To ensure scoring is updated correctly, all OKRs that are CTO aligned should be children of the CTO-level OKRs.
The Department OKRs directly aligned to the CTO-level OKRs must be updated manually or automatically from its children.

If your department has OKRs that are aligned to *CEO OKRs* that are not CTO aligned, follow the guidelines in this section, then [CEO alignment](/company/okrs/#how-to-align-division-okrs-to-the-ceo-okrs).

Using a hypothetical example:

1. CTO Objective 1: Grow the team. == Objective
    1. KR 1.1: Hit hiring target of 30 new hires. == Child objective
        1. Development: Hire 15 new hires. == Child objective
            1. Dev: Hire 5 new hires. == Key result
            1. Ops: Hire 5 new hires. == Key result
            1. Sec: Hire 5 new hires. == Key result
        1. Support: Hire 5 new hires. == Key result
        1. Infrastructure: Hire 10 new hires. == Key result

In this example, Infrastructure has 1 Director who wants to track hiring in their sub-department, so they create a separate GitLab objective with KRs for each manager.
However, the objective would not be a child of the Infrastructure "10 new hires" because they are only hiring 3 of the 10 roles. Without the other 7, it would not rollup the score correctly.
The description of the Infrastructure key result and the sub-department objective can have links to each other.

### Tracking joint OKRs

Joint OKRs across different divisions must be duplicated with one OKR item in each division. Each OKR should be aligned for scoring to each C-level (for example, one for CTO and one for CProdO for an Engineering-Product joint OKR). Titles can vary for joint OKRs, but otherwise, follow the duplicating guidance below.

For Engineering-Product joints:

1. Generally the Product OKR will be the SSoT with regular _detailed_ progress reports.
1. Ensure the Eng OKR has the `vp-development` label if the VP of Development needs to track on it.

### Tracking department OKRs

If you would like a video walkthrough, team members can view [this private video](https://youtu.be/MkKRyuhDYtE).

As GitLab objectives can only have one parent, there are various options to track OKR progress for a specific department, sub-department, or team:

1. Duplicate OKRs.
    - If you duplicate a work item, copy the wording of the title exactly. In both, ensure the description has cross-links with an indication of which one is the [SSoT](../../values/#single-source-of-truth). When updating, change the % completed on both OKRs, with a status report on the SSoT.
    - Example: See next section.
1. Track CTO aligned and non-CTO aligned OKRs separately, using assignee or label(s) to pull a list of all relevant objectives.
    - Example: [FY24-Q1 Customer Support](https://gitlab.com/gitlab-com/gitlab-OKRs/-/issues/?state=all&milestone_title=FY24-Q1&label_name%5B%5D=Department%3A%3ACustomer%20Support)
1. Don't create department objectives and track on department KRs only. Recommend using a label to pull relevant KRs.
    - Example: [VP Development label](https://gitlab.com/gitlab-com/gitlab-OKRs/-/issues/?state=all&milestone_title=FY24-Q1&label_name%5B%5D=vp-development)
1. Track only in linked epic or issue.
    - It is common that work is tracked in a `gitlab-org` issue or epic. While the OKR % needs to be updated in the OKR project, overview and all status updates could reside in the linked issue or epic.

#### Example: Duplicating OKR for tracking

Using the hypothetical example from the previous section, Development may want to track hiring at the department level.
If using the duplication method, the structure may look something like this:

1. CTO Objective 1: Grow the team. == Objective
    1. KR 1.1: Hit hiring target of 30 new hires. == Child objective
        1. Development: Hire 15 new hires. == Key result, Description links to Development 1.1 for progress updates
        1. Support: Hire 5 new hires. == Key result
        1. Infrastructure: Hire 10 new hires. == Key result
1. Development Objective 1: Grow the team. == Objective
    1. KR 1.1: Hire 15 new hires. == Child objective, Description notes % also needs to be updated in CTO 1.1.1
        1. Dev: Hire 5 new hires. == Key result
        1. Ops: Hire 5 new hires. == Key result
        1. Sec: Hire 5 new hires. == Key result

## OKR Status

- Update the OKR issue **whenever you have additional information** so that the status has the current state of the OKR.
- For direct reports of the CTO, expect to give an update in **each weekly 1:1**.
- For individuals that do a **monthly key review meeting**, expect to give an OKR update there.

At this time, there is no automatic scoring from GitLab issues. All OKRs need to be updated either manually or through rollup scoring.

## OKR Retrospection

This process should begin on the first day of the subsequent quarter, and complete no later than two weeks after.

1. After the end of each quarter, OKR owners should ensure their OKR/KR(s) progress is accurate before retrospection and closing.
1. Each OKR owner should add retrospection notes closing out their OKR/KR(s).
   1. OKR owners should retrospect as comments following our retrospection [guidelines](../workflow/#retrospective) (good, bad, and try).
   1. It's recommended that OKR owners document retrospection at the OKR (parent object) to optimize the number of retrospections/roll-ups.
1. OKR owners should review with their manager in the next 1:1 and they should discuss and close the OKR/KR(s) synchronously.
1. Managers can summarize their retrospections by closing each KR (child object) aligned to their OKR (parent object) and leaving a brief "Good/Bad/Try" in the Closing Note.
   1. If retrospection notes for KR(s) assigned to your direct report(s) have not been populated, please `@` mention your direct report DRI and ensure retrospection is captured in that OKR object.
1. After the [OKR Restrospective Meeting](../#okr-retrospective-meeting), once all outstanding conversations have been documented & applicable action items assiged to DRI(s), the leaders of each departments will ensure closure of all department's OKR/KR(s).

### OKR Retrospective Meeting

The Chief Technology Officer and the leaders of each department meet synchonously on the second Tuesday in the month after each quarter ends to [discuss the OKRs from the previous quarter](https://drive.google.com/drive/search?q=Engineering%20OKR%20Retrospective). This is an opportunity to collaborate on cross-functional initiaties with the focus being the retrospective. Leaders will voice-over the good, bad and try items from the past quarter. The meeting will not cover the status and scores of the OKRs.
