---
layout: handbook-page-toc
title: Triage Rotation
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Triage Rotation

Application Security team members are alphabetically assigned as the
responsible individual (DRI) for incoming requests to the Application
Security team for a given calendar week in the [Triage Rotation](https://docs.google.com/spreadsheets/d/18vz84dgTfetTaBjbOCXaLKNfzLYMiy_tBW6RfEUYYHk/edit?ts=5ce48702#gid=0)
Google Sheet in the Security Team Drive.

One application security engineer is assigned this task each week and can be found at [Triage Rotation](https://docs.google.com/spreadsheets/d/18vz84dgTfetTaBjbOCXaLKNfzLYMiy_tBW6RfEUYYHk/edit?ts=5ce48702#gid=0).

The following rotations are defined:

- (Weekly Assignment) HackerOne + Security Dashboard Review
    - Point of contact for "New" HackerOne reports during that week.
    - Responsible to escalating to other team members and management if the size of
    the either queue spikes.
    - Responsible for reviewing [security dashboards](https://about.gitlab.com/handbook/security/security-engineering/application-security/runbooks/security-dashboard-review.html) on a best-effort level
- (Weekly Assignment) Triage Rotation (mentions and issues)
  - First responder to mentions of the following group aliases:
    - @gitlab-com/gl-security/appsec on GitLab.com
    - @appsec-team in Slack
  - First responder to automated messages posted in the `#public_merge_requests_referencing_confidential_issues` Slack channel
    - Add a check mark emoji if the merge request can be public
    - If the merge request references a legitimate security issue
      + If the issue has a `~security-fix-in-public` label, indicating it [has been approved by an AppSec team member to be fixed in public](https://about.gitlab.com/handbook/security/security-engineering/application-security/vulnerability-management.html#fixing-in-public), link to the comment granting approval or include a message in Slack denoting that the `~security-fix-in-public` label was added.
      + Decide if it can be public anyway, and apply the fix in public label retrospectively
      + Otherwise contact SIRT and the merge request author to get the merge request removed.
      + Use the `Urgent - SEOC should be paged right away` option if waiting up to 24 hours for a resolution would be too long.
  - First responder for issues created needing triage: [~security-triage-appsec issue search](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name%5B%5D=security-triage-appsec)
    - Refer to [this page](https://about.gitlab.com/handbook/security/#reproducibility-on-security-issues) to learn about the different labels that we can apply to issues when they're not vulnerabilities
  - First responder to [JiHu Contribution pings](https://about.gitlab.com/handbook/ceo/chief-of-staff-team/jihu-support/jihu-contribution-review-process.html) that come into the `#sec-appsec` Slack channel
- (Monthly Assignment) Security Engineer for Security Releases
- (Monthly Assignment, Federal AppSec only) Release Certifications
  - Responsible for the [release certification process](https://about.gitlab.com/handbook/ceo/chief-of-staff-team/jihu-support/release-certification.html)
  - This applies to any release that might have JiHu contributions, including monthly and patch releases
- (Quarterly Assignment) Bug Bounty/AppSec Blog Post

If the Application Security team member has a conflict for the assigned week
they may swap rotation weeks with another team member. This may be done for
any reason including time off or the need for time to focus on a particular task.

Team members should not be assigned on weeks they are responsible for the
scheduled security release.

Team members not assigned as the DRI for the week should continue to triage
reports when possible, especially to close duplicates or handle related reports
to those they have already triaged.

Team members remain responsible for their own assigned reports.
