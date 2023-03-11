---
layout: handbook-page-toc
title: "Core Team"
---

{::options parse_block_html="true" /}

## On this page

{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Becoming a Core Team member

A new member can be added to the [Core Team](/community/core-team/) at any time through the following steps:

1. Current Core Team members can nominate a new member from the wider community at any time using a confidential issue in [the Core Team group](https://gitlab.com/groups/gitlab-org/gitlab-core-team/-/issues).
2. The nominee will be added to the Core Team if they have received positive votes from two-thirds (2/3) of all current core team members within a two week period and accept the nomination.
3. Once a new member has been added, start the onboarding process by following the steps outlined in the [Core Team member orientation section](/handbook/marketing/community-relations/code-contributor-program/core-team/#core-team-member-orientation) below.
  
## Monthly Core Team meetings

The Core Team meets on the third Tuesday of each month and anyone is welcome to join the call.
Call logistics/agenda/notes for the meeting are available on the [Core Team issue tracker](https://gitlab.com/gitlab-org/gitlab-core-team/general/-/issues).
All meeting recordings are available at the [Core Team meeting Playlist](https://www.youtube.com/playlist?list=PLFGfElNsQthZ12EUkq3N9QlThvkf3WGnZ).

## Contacting Core Team members

Core Team members can be reached by [mentioning](https://docs.gitlab.com/ee/user/group/subgroups/index.html#mentioning-subgroups) `@gitlab-org/gitlab-core-team` in issues or merge requests.

While GitLab is the primary means of contact, the Core Team can also be contacted on the [#core](https://gitlab.slack.com/messages/core) Slack channel.

Anyone can open an issue in the [Core Team issue tracker](https://gitlab.com/gitlab-org/gitlab-core-team/general/-/issues).

## Offboarding and stepping down gracefully

If you are no longer able to or interested in serving in the Core Team, you should make an announcement on the `#core` Slack channel. When you step down, you will become a [Core Team Alumni](/community/core-team/alumni/). Once a Core Team member steps down, GitLab team member(s) will start the off-boarding activities to:

1. Move the individual from the `team.yml` file to the `alumni.yml` file.
2. Create an issue in [team-member-epics/employment](https://gitlab.com/gitlab-com/team-member-epics/employment/-/issues) using the [`offboarding` template](https://gitlab.com/gitlab-com/people-group/employment-templates/-/blob/main/.gitlab/issue_templates/offboarding_core_team_member.md) and fill out the "Core Team Members" section to remove the individual from GitLab Slack, [the Core Team Group](https://gitlab.com/groups/gitlab-org/gitlab-core-team/community-members/-/group_members), gitlab-org etc.

## Core Team Member Orientation

1. Email the nominated member to confirm they are interested before beginning the orientation process.
1. Create an issue in the [Lifecycle Management Project](https://gitlab.com/gitlab-com/temporary-service-providers/lifecycle) using the [Core Team Member Orientation Issue Template](https://gitlab.com/gitlab-com/temporary-service-providers/lifecycle/-/issues/new?
issuable_template=orientation_issue_core_member) and follow the steps outlined.
  - Core team members must sign an NDA before granting them any access.
1. Create a public issue in the [Core Team Project](https://gitlab.com/gitlab-org/gitlab-core-team/general/-/issues/111) including the steps (as found in the Core Team member Orienation Issue Template) the new team has to take.

## Core Team Group

All Core Team members are part of the [`gitlab-org/gitlab-core-team`](https://gitlab.com/gitlab-org/gitlab-core-team/) group on GitLab.com. This group has a particular structure for specific automation purposes:


```mermaid
graph TD
    A("gitlab-core-team (group)<br>-Has both GitLab team and wider community Core Team members-") --> B("community-members (group)<br>-Has only wider community Core Team members-")
    A --> C["general (project)"]
```

The [`community-members`](https://gitlab.com/gitlab-org/gitlab-core-team/community-members) group exists to:

* [facilitate triaging](https://gitlab.com/gitlab-org/quality/triage-ops/-/merge_requests/65) and;
* [ensure Core Team members are credited in the changelog](https://gitlab.com/gitlab-org/gitlab/-/merge_requests/69076)

## Core Team member benefits

As part of the trust, value and recognition that joining the Core Team implies, each member is granted a number of benefits to support them in their contributions.

### Slack access

Core Team members are granted [access to the GitLab team's Slack instance](/handbook/tools-and-tips/#channels-access) as part of their [Core Team Member Orientation](#core-team-member-orientation).

A list of the up-to-date channels the Core should/have access to can be found in the [Core Team and Slack](https://docs.google.com/spreadsheets/d/1kohQBbvk2JSl3DXrmF5TDsWVoAMi_yujFWzzAP6vq2M/edit#gid=0) Google Sheets and in the list below:

<style>
.display-inline-block {
  display: inline-block;
}
</style>

<details>

<summary>

#### Slack channels Core Team can access
{: .display-inline-block}

</summary>

- development
- gdk
- mr-coaching
- quality
- community-relations
- backend
- frontend
- frontend_pairs
- is-this-known
- gitter-contributors-room
- gitpod-gdk
- database-lab
- docs
- triage
- linux
- g_runner
- golang
- community-hangout
- community-relations-fyi
- community-programs
- developer-evangelism
- cfp
- fosdem
- master-broken
- review-apps-broken
- qa-master
- qa-nightly
- qa-preprod
- qa-production
- qa-staging
- triage-automations
- backend_maintainers
- frontend_maintainers
- lang-ru, lang-jp
- opensource
- docs-tooling
- production
- competition
- gck
- website
- vim
- tw-team
- g_engineering_productivity
- mr_feedback
- backend_pairs
- f_graphql
- f_rubocop
- database
- product
- jetbrains-ide
- design-system
- ux-coworking
- office-today
- remote
- questions
- lang_ru
- lang_jp

</details>

<details>

<summary>

#### Slack channels Core Team cannot access
{: .display-inline-block}

</summary>

- release-post
- security
- questions
- connect-to-contribute
- all-caps
- random
- whats-happening-at-gitlab
- thanks
- diversity_inclusion_and_belonging
- company-fyi
- contribute2021
- ux

</details>

#### Requesting Core Team access to Slack channels
1. Please submit an [access request](https://gitlab.com/gitlab-com/team-member-epics/access-requests/-/issues/new?issuable_template=Individual_Bulk_Access_Request) with the new channel(s) requested.
1. Assign the issue to the [Code Contributor Program Manager](https://about.gitlab.com/handbook/marketing/community-relations/code-contributor-program/#contact) who will complete the next steps.
1. Code Contributor Program manager to: Identify the channel(s) owner and invite them to review the request by leaving a comment on whether they agree on having Core Team members in their channel(s).
1. (no action needed) After successful review, issue is handed/assigned to Slack Admins, for inviting Core Team members to the channels.

All the channels Core Team members have access to, should follow the [SAFE guidelines](https://about.gitlab.com/handbook/legal/safe-framework/) when posting in the channel. Even though the Core Team Members have signed an NDA, they are not considered GitLab team members.

### Developer permissions for GitLab projects

To improve their development experience, Core Team members are granted [`Developer` permissions](https://docs.gitlab.com/ee/user/permissions.html#group-members-permissions) on the [`gitlab-org` group](https://gitlab.com/gitlab-org), where the vast majority of projects for GitLab (the product) reside. For any project under that group, and among other abilities, this enables them to:

- Create branches on the source project instead of forks
- Assign merge requests
- Assign issues
- Manage and assign labels

At this time, Core Team members are not added to the [`gitlab-com` group](https://gitlab.com/gitlab-com), which is used for projects and processes associated to the GitLab company.

The Code Contributor Program Manager will generally take the action to grant this permission as part of the new Core Team member's orientation issue.

### Team page listing

To emphasize their affiliation and closeness to the GitLab team, and to raise visibility on their profile, Core Team members can [add themselves to the GitLab team page](/handbook/git-page-update/#12-add-yourself-to-the-team-page) via the Code Contributor Program Manager (who will be able to merge the MR).

This will list their profile on [the Core Team page](/community/core-team/) as well.

### GitLab top tier license

To enable contributions and to gain insight on GitLab capabilities, Core Team members can [request a free top tier license for development purposes](/handbook/marketing/community-relations/code-contributor-program/#contributing-to-the-gitlab-enterprise-edition-ee) via the Code Contributor Program Manager.

GitLab top tier licenses in SaaS or self-managed instances are granted to Core Team members for 1 year and can be renewed for another year during the Core Team member term. If a member decides to step down but still wishes to contribute to GitLab occasionally, they will still be eligible for a GitLab license, but the renewal period will be the [standard 3 months given to other GitLab community members](/handbook/marketing/community-relations/code-contributor-program/#contributing-to-the-gitlab-enterprise-edition-ee).

There is no specific limit on the number of seats that Core Team members can request. We trust Core Team members to use their own judgement to estimate the number of users they will need for development purposes, and not to use the license for for-profit purposes.

### JetBrains license

To support their code contributions to GitLab, Core Team members can [request a JetBrains license for development purposes](/handbook/tools-and-tips/other-apps/#jetbrains) via the Code Contributor Program Manager.

### Sponsored access to GitLab events

To support contribution at in-person or virtual events, Core Team members will be eligible for sponsored access (subscription, accommodation, travel) to GitLab events (e.g. GitLab Contribute, GitLab Commit).

### Personalized merchandise

On occasion, the GitLab team might offer personalized merchandise exclusive to Core Team members to contribute in style!
