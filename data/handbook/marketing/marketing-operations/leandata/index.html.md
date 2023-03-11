---
layout: handbook-page-toc
title: "LeanData"
description: "LeanData is an application used within Salesforce (SFDC) to process and assign lead, contact, and account records."
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview     
LeanData is an application used within Salesforce (SFDC) to process and assign [lead](#lead-routing-workflow), [contact](#contact-routing-workflow), and [account](#account-routing-workflow) records. LeanData allows for the creation of dynamic and complex record routing to support Go-to-Market (GTM) strategy.  

LeanData assigns each MQL (Marketing Qualified Lead) to the member of the Sales Development organization who is responsible for engagement and qualification of that individual using the [lead routing workflow](#lead-routing-workflow) outlined below. LeanData updates contact records using the [contact routing workflow](#contact-routing-workflow) for management by partners via the Vartopia Prospect module. LeanData align, but does not assign, each account record to the appropriate member of the Sales organization using the [account routing workflow](#account-routing-workflow) outlined below. Other Salesforce objects, including for most use cases the contact object, are updated and maintained through workflows and processes outside of LeanData. 

## Lead routing workflow
The LeanData lead routing flowbuilder can broken into four major sections: [record validation](#record-validation), lead to account match MQL assignment, [unmatched MQL assigment](#unmatched-lead-mql-assignment), and [queue assignment](#queue-assignment). This flowbuilder is live, meaning it monitors lead records as they're created or updated. 

### Record validation
This initial phase reviews new and updated lead records to ensure they meet the criteria to route to an SDR. These checks include confirming:
- [New leads only] Lead record was created by an integration user and the `Do Not Route?` checkbox is not checked.
- [New leads only] `Person Score` of the lead record is greater than or equal to 0. Note this means leads without a `Person Score` or leads that have a `Person Score` less than 0 will continue to be owned by the integration user that created the record. Also, the current `Person Score` threshold is a change from previous routing rules and at the moment, only impacts new leads, not historically created records.
- [New leads only] Company information is available and records missing company data have a standardized response in the `Company` field.
- [Updated leads only] No active SDR engagement with the lead. This is checked by confirming the lead does not have a `Lead Status` of `Accepted`, `Qualifying`, or `Qualifed` and the `Actively Being Sequenced` checkbox is not checked.
- [New and updated leads] Most recent `Last Interesting Moment` does not require specialized routing or supression from SDR organization.

### Sales Dev lead assignment
#### Lead to account match MQL assignment
Records that meet all [record validation](#record-validation) criteria and can be matched to an existing Salesforce account by LeanData are then assessed using the matched account workflow. For this workflow, if LeanData is able to identify there is a BDR listed in the `BDR Assigned` field on the matched account and the `BDR Prospecting Status` (another custom account field) = `Actively Working`, the MQL is assigned. If LeanData is not able to confirm an MQL matches this criteria, the lead progresses to the [unmatched lead](#unmatched-lead-mql-assignment) workflow.

#### Unmatched lead MQL assignment
Leads that match to accounts but are not able to be routed via owner mappings or the `SDR Assigned` field as well as leads that do not match to accounts are routed by country assignment.

#### Queue assignment
Leads that are not yet MQLs or that are no longer being worked by the Sales Development team, are assigned to "holding" queues until they re-MQL. 

Leandata runs a weekly job that looks for leads in `Recycle`, `Bad Data`, `Ineligible`, `Inquiry`, and `Disqualified` statuses, not in an active sequence, and owned by a Sales Dev user and reassigns the lead to the appropriate queue based on status. 

#### Exceptions to these rules
##### US PubSec lead assignment
US PubSec leads are assigned to US PubSec BDRs regardless of `Lead Status`, if they have been identified as part of a US PubSec account. This is an exception to our standard lead management process where non-US PubSec leads that have not yet MQLed would be assigned to a [queue](#queue-assignment) until that condition is met.  

### Partner lead management (via the Vartopia Prospect module)
#### MDF Campaign
New and updated campaign members acquired by an [MDF Funded Campaign](https://about.gitlab.com/handbook/marketing/channel-marketing/partner-campaigns/#partner-only-campaigns---mdf-funded) is routed to the lead flowbuilder.

1. LeanData reviews for the campaign field for `Will there be MDF funding` = `Yes`.
1. LeanData updates the `Prospect Share Status` = `Sending to Partner` and `Partner Propsect Status` = `Qualifying` which enables the lead to be synced into the Vartopia Prospect module.
1. LeanData assigns the lead to `Partner Queue` if `Partner Account` is `NULL`.

#### Self-Managed Free Trial

New and updated campaign members acquired by [Partner Managed Trial](https://about.gitlab.com/handbook/marketing/channel-marketing/partner-campaigns/#trials-from-partners) is routed to the lead flowbuilder.

1. LeanData reviews for the campaign name for `Partner - Trial - Self-managed`.
1. LeanData updates the `Prospect Share Status` = `Sending to Partner` and `Partner Propsect Status` = `Qualifying` which enables the lead to be synced into the Vartopia Prospect module.
1. LeanData assigns the lead to `Partner Queue` if `Partner Account` is `NULL`.

#### Joint Events with Partners

New and updated campaign members acquired by attended a [Joint GitLab and Partner Event](https://about.gitlab.com/handbook/marketing/channel-marketing/partner-campaigns/#joint-gitlab-and-partner-events) are routed to the lead flowbuilder.

1. LeanData reviews the campaign fields for `Is a Channel Partner Involved?` = `Yes` and `Campaign Member Status` with regards to partner engagement.
1. LeanData verifies the campaign member is not actively worked by GitLab, thus `Person Status` is not `Accepted`, `Qualifying` nor `Qualified`, or `Actively Being Sequenced` = `False`.
1. If all above is
    1. True, then LeanData updates the `Partner Prospect Status` to `Qualifying`, `Prospect Share Status` = `Sending to Partner`, then LeanData assigns the lead to `Partner Queue`
    1. False, then LeanData assigns to appropriate SDR.

#### Exceptions to this rule
When a lead/contact engages with GitLab in any shape or form, for example, via an inbound marketing request, the lead/contact owner is responsibility for following up with the partner lead, regardless of their stage within the partner lead lifecycle.

## Contact routing workflow
The scope of the contact flowbuilder is very limited. Records are only processed by this flowbuilder if they are meant to be managed by partners via the Vartopia Prospect module. In our current iteration, the contact flowbuilder only updates two custom fields, which triggers a partner's record visibility in Vartopia. 

All other [SFDC contact ownership rules](https://about.gitlab.com/handbook/sales/field-operations/gtm-resources/#changing-contact-ownership-in-salesforce) are maintained outside of LeanData. If you have questions or concerns about contact routing outside of partner record management processes, please reach out to [Sales Systems](https://about.gitlab.com/handbook/sales/field-operations/sales-systems/).

## Account routing workflow
The account routing flowbuilder leverages LeanData's territory management functionality to populate or update the `[TSP] Territory`, `[TSP] Region`, `[TSP] Sub-Region`, `[TSP] Area`, and `[TSP] Approved Next Owner` fields on the account object. LeanData monitors for changes to the `[TSP] Last Update Timestamp` field to know when an account record is ready to be processed. Details about the TSP process can be found on the [Sales Operations handbook page](https://about.gitlab.com/handbook/sales/field-operations/sales-operations/#territory-success-planning-tsp). 

## Lead routing request or question?

### Request an SDR alignment update
New hire? Territory change needed? Have an SDR on your team who's going to be out of the office? If requesting a proactive update to the lead routing workflow, open an issue using the [LeanData change request issue template](https://gitlab.com/gitlab-com/marketing/marketing-operations/-/issues/new?issuable_template=leandata_change_sdralignment).

### Experiencing a lead routing problem?
Lead volume low? Receiving leads from an account or territory you're not assigned to? If you think you've found a bug :bug: in existing lead routing logic, open an issue using the [bug request issue template](https://gitlab.com/gitlab-com/marketing/marketing-operations/-/issues/new?issuable_template=bug_request). 

### General questions
Open a [Marketing Operations issue](https://gitlab.com/gitlab-com/marketing/marketing-operations/-/issues/new) following the format in the issue template.


## LeanData Lead Flow Update Process

- Every Monday, create a clone of the Live Lead Routing flow and name it " LIVE ON following Monday's Date: Summary of edits" - Eg "Live on 12/12: Related Campaign Member/Distribution edits"

- This logic will be the flow that everyone adds their updates to for the week (if any).

- If you need to play around with the logic/your updates will take longer than a week to build, create a separate clone to do so and then add the final edits into the next draft that will go live.

- If there are any urgent updates needed, make the draft flow live, but create a new clone for people to continue working on.

