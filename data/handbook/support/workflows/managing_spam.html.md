---
layout: handbook-page-toc
title: Managing Spam
description: "Instructions for flagging/unflagging suspicious Issues, and deleting abusive user accounts on GitLab.com"
category: GitLab.com
subcategory: Security
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

### Flagging Issues as Spam

Many spammers use GitLab.com to create spam. Starting with 8.11, GitLab has
better integration with Akismet to check for spam whenever a user creates an
issue. This filter needs to be trained properly, however. With some effort our
spam detection should improve. If an issue is created on GitLab.com by a
spammer, before deleting the account, flag the user's issues as spam:

1. Login to GitLab.com with an admin account
2. View each issue and click on "Submit as spam"

Where multiple issues are created or commented on,
GitLab team members can also report spam in the #abuse Slack channel by tagging the `@trust-and-safety` team.

### Deleting Spammers

Once the issues are flagged and the user is verified to be a spammer, go to
the spammer's user profile and click on the "Report Abuse" button:

1. Login to GitLab.com with an admin account
2. Go to: https://gitlab.com/admin/abuse_reports
3. Be careful: Click on "Delete user" only if you are sure this user is a spammer.

### False positives: Ham

Both the Akismet filter and [Spamcheck](https://gitlab.com/gitlab-com/gl-security/runbooks/-/blob/master/automation/spamcheck.md) may also flag false positives and prevent a user from
creating issues. The contents of the flagged issue get stored in the spam logs,
which is only accessible to admin users. If you're unsure whether Akismet or Spamcheck is disrupting the creation of artifacts(issues, snippets, etc) you may diagnose the problem as described in the [Security runbook entry for falsely labelled spam](https://gitlab.com/gitlab-com/gl-security/runbooks/-/blob/master/automation/spamcheck.md#false-negative-and-false-positive-investigation).

From time to time, we may need to submit the flagged issue as "ham" (e.g. when a user lodges a complaint on the
Support Tracker about not being able to create issues). Currently, there are
no notifications whenever an entry is flagged, so this needs to be monitored
periodically. To flag an issue as ham:

1. Login to GitLab.com with an admin account
2. Go to: https://gitlab.com/admin/spam_logs
3. Scan the contents of each log. If it appears that a user is trying to post valid
   information, click on "Submit as ham".

### More Advanced Spam Fighting

At times GitLab.com can appear overrun by specific types of spam. Spammers often
target public snippets, projects, issues, and merge requests for advertising
their wares. Details on more advanced spam fighting techniques can be found in
the [internal GitLab-only Spam Fighting Google Doc](https://drive.google.com/drive/u/0/search?q=%22Spam%20fighting%20runbook%22).
