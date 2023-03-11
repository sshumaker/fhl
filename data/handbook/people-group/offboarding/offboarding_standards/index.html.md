---
layout: handbook-page-toc
title: "GitLab Offboarding Standards"
description: "Offboarding process and steps on the backend"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

{::options parse_block_html="true" /}

<div class="panel panel-gitlab-orange">
**This is a Controlled Document**
{: .panel-heading}
<div class="panel-body">

Inline with GitLab's regulatory obligations, changes to [controlled documents](https://about.gitlab.com/handbook/security/controlled-document-procedure.html) must be approved or merged by a code owner. All contributions are welcome and encouraged. 

</div>
</div>

# GitLab Offboarding Standards

## Purpose
These standards specify requirements related to the offboarding of GitLab team members from all GitLab related computing resources and data assets so as to protect our customers, team members, contractors, company, and other partners from harm caused by both deliberate and inadvertent misuse. Our intention in publishing these standards is to outline information security standards intended to protect GitLab assets.

## Scope
These standards apply to all GitLab team-members, contractors, advisors, and contracted parties interacting with GitLab computing resources and accessing company or customer data.

## Roles & Responsibilities:

| Role  | Responsibility | 
|-----------|-----------|
| GitLab Team Members | Responsible for following the requirements in this document |
| PeopleOps | Responsible for implementing and executing this document | 
| PeopleOps (Code Owners) | Responsible for approving significant changes and exceptions to this document |

## Offboarding Procedure

### Notice of Offboarding

Once the termination process has been approved and completed in Workday either by the departing team members [Direct Manager](https://docs.google.com/document/d/1Fr1G1i1kssfADgDf3D6LbZHR8RZmWKZYDNV8AfduZ1c/edit) (Voluntary) or by [Team Member Relations](https://docs.google.com/document/d/1nMokz03AiUQtb0XV5zpD9CjaQKcX5Lu8p5ASZy3cJVA/edit) (Involuntary) either a People Connect (Voluntary) or Team Member Relations (Involuntary) team member will submit an [Offboarding Workflow Form](https://docs.google.com/forms/d/e/1FAIpQLScBBnV7bKKVkqfTk9Aq9sfSB_r85SKTxt0_mC6RhbRwU3DtSA/viewform).  In the instance of a Voluntary Termination this process will follow the [resignation process](https://docs.google.com/document/d/1AVHHBKd6dtyn0DOl4_UydbdEhectLpH5aMh17r9Sg_4/edit) intiated by the team member directly in Workday.

This will populate the tracker through which various offboarding automations are triggered in addition to notifying IT Operations; Payroll and other Stakeholders of the team members temination particulars such as the effective date, information about garden leave if applicable and the time at which access to GitLab systems should be terminated in the #offboarding channel.

In alignment with the needs of both People Connect and IT Operations, offboardings will kick off at 16:00pm in the team members regional timezone (EMEA, JAPAC, and NORAM) and 12:00pm in their regional timezone on Friday at which point de-provisioning will commence.

**Note:** In instances where team members require de-provisioning initiated at outside of those documented above they should reach out to People Connect via direct message or people-connect@gitlab.com to arrange an alternate time.

Should the effective date fall on a day which People Connect is unable to support e.g. a Family and Friends Day or Global Holiday, People Connect will reach out to the People Business Partner to discuss alternate offboarding options. 

### Offboarding Assignments

Per the People Connect Rotation the offboarding will be assigned directly in the [offboarding tracker](https://docs.google.com/spreadsheets/d/1Z45eOZ2rCRIKgGae3eOKQ8lhIbAPikSs5gLz3V8Kh9U/edit?ts=5e7a2c42#gid=989170380). 

### Creating the Offboarding Issue

Offboarding issues are created [automatically](https://about.gitlab.com/handbook/people-group/engineering/offboarding/#scheduled-offboarding-issue-creation) using the data that is populated by the offboarding form. **It is essential that the date and time inserted in the tracker is accurate as this will be the time at which the employment bot will open the offboarding issue**

The assigned People Connect member will be automatically added to the list of assignees once the offboarding issue is created.

Many teams work to deprovision access including the IT Operations, this should be regarded as urgent and all tasks expected to be completed in 5 working days with the exception of [laptop returns](/handbook/business-technology/team-member-enablement/onboarding-access-requests/#returning-oldoffboarded-laptops), which can take 2 - 4 weeks.

Note: If the team member is temporarily transitioning to a [contractor or consultant role](/handbook/people-group/general-onboarding/consultants/), please proceed with the full offboarding process and create a separate onboarding issue to grant only specific temporary access for what they would need to fulfill their contractual obligations.

#### Creating the Offboarding Issue Manually

In the event that the offboarding issue is not automatically opened or an urgent issue is needed to be opened, the People Connect member can open the offboarding issue manually, by following the steps below:

1. In Slack, go to your profile as if you were going to send a Slack message to yourself. Type the command `/pops run offboarding <EMPLOYEE_NUMBER>`.
1. You will be pinged in Slack once the offboarding issue is created, which usually takes 30 seconds or so. The ping will include a link to the offboarding issue and merge request removing from team page.
1. You will need to check the Department, GitLab Email Address and GitLab Handle within the issue are correct.

### Offboarding Tools

#### Google Workspace

IT Ops will follow the below steps to set up an auto-response that notifies the sender that the team member they are trying to reach is no longer with GitLab and who to contact.

   1. Navigate to Google admin portal and search for the email account.
   1. Unsuspend the account, reset sign in cookies, reset password, do not email the password. 
   1. Move account into the Former Team Memebers Organizational Unit. 
   1. Use GAM to set a Out of Office Message on the account
   1. Add the [appropriate template](https://gitlab.com/gitlab-com/people-group/people-operations/employment-templates/-/blob/main/email_templates/offboarding_rejection.md) per team member's department under the `Customize rejection notice`

The Out of Office message will stay on the account for 90 days, aftewards ITOPs will follow up and archive the account in the G-Suite vault.

#### Slack

- Bots

IT Ops check if the team member has created any bots before disabling the account. Go to [Slack](https://gitlab.slack.com/apps/manage) or on your admin Slack profile click Menu >> Configure Apps >> Custom Integrations >> Bots and search through the bots' list for the team member.
If a bot exists, please DM the manager to confirm if the bot should be removed.

#### Team Page

As per the [automation](https://about.gitlab.com/handbook/people-group/engineering/offboarding/#offboarding-merge-request) in place, a merge request is automatically created to remove the team member from the team page. This will update the following:

- Removing the individual file from the data/team_members/person directory
- Removing the picture used in the previous file
- Adjusting the reports_to in case the offboarded team member had reports
- Removing the pet picture in case the team member had any
- Removing the pet page entry
- Update the CODEOWNERS file: change to the manager or remove if the manager is already a codeowner for that file

The People Connect Team member will need to complete:

- Remove the team members ReadMe

### Offboarding Compliance

The People Connect Team member in the relevant rotation will complete a weekly audit of all offboarding issues opened within that specific week and check that all tasks have been completed by all Team Member and/or Departments. In the event that tasks are still outstanding, the People Connect Team member will ping the relevant Departments within the offboarding issue to call for tasks to be completed.

Once all tasks have been completed, the People Connect Team member will close the offboarding issue and mark as completed in the offboarding tracker.

All offboarding tasks by all Departments need to be completed within 5 days of the offboarding date. For systems that are more critical and time sensitive, these will be completed within the first 24 hours (example 1Password, Slack) by the relevant Departments. Information about application & system deprovisioners can be found on the [Tech Stack Applications handbook page](/handbook/business-technology/tech-stack-applications/).

To ensure a successful completion of the offboarding issue, it is important that all tasks are checked off, whether the system/tool is applicable to the offboarding team member or not. Checking the box indicates one of the following:

- I have revoked team member access to this particular system/tool
- I have checked and this team member was not given access to this particular the system/tool

## Exceptions
Exceptions to this policy must be approved by PeopleOps.

## References
* [Information Security Parent Policy](/handbook/security/)
* [GitLab Offboarding](https://about.gitlab.com/handbook/people-group/offboarding/)
* [GitLab Offboarding FAQ](https://about.gitlab.com/handbook/people-group/offboarding/faq.html)
