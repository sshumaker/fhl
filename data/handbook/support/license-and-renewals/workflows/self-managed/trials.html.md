---
layout: markdown_page
title: Handling trials and extensions for GitLab Self-Managed
category: GitLab Self-Managed licenses
description: Issuing a license to "extend" Self-managed trials and grace periods
---

{:.no_toc}

----

## Overview

Self-managed trials and grace periods cannot be extended - a **trial** license
must be issued and applied to the instance in order to "extend" a license.

Requests for grace period extensions, temporary keys, temporary extensions, temporary licenses, 
and trial extensions all require generating a trial License.

Sales will often request through a [Zendesk Ticket](https://gitlab-com.gitlab.io/support/internal-requests-form/) that we extend the duration of Self-Managed trials on behalf of their prospects. These tickets will always be raised from the GitLab Support End User gitlab_support@example.com, with the submitter cc'd on the ticket. The following workflow should be followed to service them.

If any fields when opening the ticket were filled out incorrectly, send a public reply in the ticket asking the submitter to supply the missing information.

> **NOTE**: Non-trial licenses are required to match an existing subscription and these licenses 
generally have a span of 1 year. There is an 
[ongoing discussion](https://gitlab.com/gitlab-com/support/support-team-meta/-/issues/3817) on
how to support complex subscription models.

Support tries as much as possible to refrain from issuing non-trial licenses.
We are allowed to issue trial licenses because they:

- Have no grace period
- Don't affect historical data tracking
- Aren't tied to any subscriptions for revenue purposes

### How to create a new trial license

Users should initiate a request on their own by clicking on the following link:  https://about.gitlab.com/free-trial/?hosted=self-managed

### How to extend an expired or soon to expire license

1. Before taking any action to create the trial license, get confirmation from
   the customer that they understand and accept the
   [constraints](https://about.gitlab.com/free-trial/#what-is-included-in-my-free-trial-what-is-excluded)
   that accompany a trial. Use the `Support::L&R::Trial Subscription - Exclusions Sign Off`
   macro in Zendesk for this purpose. Be sure to assign the ticket to
   yourself so that you will receive the customer's response and be
   able to take action quickly.
1. Open the expired or soon to expire license and select `Duplicate License`
1. Set the `License type` to `Legacy License`.
1. Delete the contents of `Zuora subscription ID` field if present.
1. Set the `Users count` number to what is requested.
1. Set the `Previous users count` number to the previous license **if there are trueups**. Otherwise, delete the contents.
1. Set the `Trueup count` number if present.
1. Set the `Plan code` to what is requested.
1. Ensure the `Trial` checkbox is checked. 
1. Set `Starts at` to today's date.
1. Set `Expires at` to the requested date. 
1. Set `Notes` to the ticket or issue URL.
1. Click `Save`. The license will be automatically sent to the email specified in the `Email` field.

If you need to [send a trial license to another contact](/handbook/support/license-and-renewals/workflows/self-managed/sending_license_to_different_email.html#overview), 
use the `Forward license email` tab after saving the new license.

### Emergency Weekend Licenses

If you're on call and you need a license generated, but don't have access to the CustomersDot interface, follow the [Weekend Emergencies - License Request](/handbook/support/license-and-renewals/workflows/self-managed/license_for_weekend_emergencies.html) workflow.

