---
layout: handbook-page-toc
title: Slack
description: Information on Slack automations created by the People Engineering team.
---

## On this page
{:.no_toc}

- TOC
{:toc}

## Integrations

For several smaller automations we use integrations with Slack. On this
page you can find an overview of all the integrations we've set up. Most
of these integrations use a Slack bot named `PeopleOps Bot`.

### Anniversary announcements

A scheduled pipeline is configured to automatically send a message
congratulating all team members celebrating a work anniversary that week to the
Slack channel [`#team-member-updates`](https://gitlab.slack.com/archives/CL55Q4U0K). The message will contain list of all such
team members and the number of years they are celebrating at GitLab.

Currently, the pipeline is scheduled to be run at 10:00 AM UTC on every
Thursday.

### Birthday announcements

Every monday morning, a scheduled pipeline is configured to automatically send a message
congratulating team members celebrating their birthday that week to the
[`#celebrations`](https://gitlab.slack.com/archives/C7RLMNSFJ) Slack channel. Only team members who have opted-into GitLab birthdays
on their Slack profile will be listed in the congratulatory message.

To opt-in, follow these steps on Slack

1. Click on your profile photo in the top right corner
1. Click on `Edit profile`
1. Scroll down to the `GitLab Birthdays` field and select `Yes`

### Parental Leave Welcome Back

A scheduled pipeline runs every day to check who's coming back from parental leave in 3 days.
For those team members we send them a Direct Message reminding them that they can take more
PTO if needed and links to the handbook related to coming back after parental leave.

For this pipeline we have a direct integration with PTO by Deel.

### Informing People Connect Team about details missing in BambooHR for upcoming new hires

For the new hire announcements to be accurate, it is required to ensure the
Workday details of team members joining the following week is as complete as
possible. To help the People Connect team in this task, another scheduled pipeline is
run to verify if the Workday details of all incoming team members is complete.
This pipeline notifies the People Connect Specialists in [`#peopleops-alerts`](https://gitlab.slack.com/archives/CLTBQ9XC7) channel
about people whose details are missing and the details that are missing for each
person.

Since the People Connect Specialists should have enough time to fix these missing
details before new hire announcements are sent, it is necessary this job should
be run an adequate amount of time before the new hire announcements job is run.
Currently, the pipeline is scheduled to be run at 02:00 PM on every Wednesday.

### Offboarding sheet

There is a Google form that People Connect submits scheduled or voluntary offboardings into, this is then stored within a Google Sheet which we check every day to determine whether or not anyone is being offboarded within the hour. This automation runs every hour to check and see if we have any new team members that are being offboarded, if there are any, we then open the related offboarding issues automatically.

### Employment survey

Whenever a team member fills in on of the following surveys, the form entrance
is put into a slack message to the private Slack channel `employment-survey`. This way the
People Connect team can discuss and take action.

- Onboarding Survey
- Values Check-In
- Career Mobility Value Check-In
- Career Mobility Satisfactory Survey

### Hiring Manager Survey
Whenever a new team member is added to a team we currently send a couple of notifications.

- `DM` - will attempt to send a survey DM to the new team members hiring manager.
- `Alert` - will send this survey as a link to the `#peopleops-alerts` channel if the DM could not be sent.

### Template Paths

People Connect associates can type `/pops run templatepaths <EMPLOYEE_NUMBER>` to output
the list of locations where the bot looks to fill-in role/specialty based access request
and onboarding tasks. This command is useful when it is unclear why an automated issue
creation did not pick up a given template. This will show exactly what path the bot expects.

### GitLab Usernames

Often times, team members won't follow the procedure outlined on the [tools and tips page](/handbook/tools-and-tips/#change-your-username-at-gitlabcom) to change their GitLab username. This leads to inaccurate or outdated data in Workday.
To remedy this situation, every Wednesday, we audit all GitLab usernames stored on Workday (`GitLab Username` field) and verify that those usernames are members of the [gitlab-com group](https://gitlab.com/groups/gitlab-com/-/group_members). When a Workday `GitLab Username` is not in the group, a message is automatically sent in `#peopleops-alerts` on Slack.
