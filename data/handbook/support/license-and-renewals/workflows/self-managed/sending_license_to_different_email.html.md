---
layout: markdown_page
title: Sending licenses to a different email address
description: "Information on the process for sending licenses to a different email address"
category: GitLab Self-Managed licenses
---

{:.no_toc}

----

## Overview

A temporary license can be sent to a different email address.

A paid license is always sent to the `Sold to` contact used on the order, and this contact is mentioned in the license file.

We can send the license to another contact if:

- The contact has a Customers Dot account which is linked to the subscription.
- The contact is the `Sold to` contact for the Zuora account.

To have it sent to a different email address, we would need to follow the process outlined at [Associating purchases with additional accounts](https://about.gitlab.com/handbook/support/license-and-renewals/workflows/customersdot/associating_purchases.html). \
We cannot bypass doing this based on internal requests. It must be done via a customer submitted ticket. \
Once the new Customers Dot account is created or changed, the license can be re-sent (or obtained by the new account owner).

The Support team is not allowed to make changes to the contact information in the license itself.

To forward or resend a license:

- Find the license by following steps 1 and 2 mentioned in the [above section](#overview). 
- To resend the license to the same user, click the `Resend to customer via email` button on the right. (Looks like an envelope icon). 
    - **Note:** For Cloud Activation codes, follow the process to [update the `Sold To` contact in Zuora](https://about.gitlab.com/handbook/support/license-and-renewals/workflows/billing_contact_change_payments.html#zuora-contact-change) before resending. ([Reference](https://gitlab.com/gitlab-org/customers-gitlab-com/-/blob/main/app/models/subscription.rb#L589)).
- To forward the license to a different address using the `Forward license email` function. 
    1. Navigate to the `Forward license email` tab. 
    1. Enter the `Destination email address`. **NOTE** It is currently not possible to copy (cc) or send to multiple contacts at once.
    1. Click the **Forward** button.
    1. [Confirm whether the license was delivered](/handbook/support/license-and-renewals/workflows/self-managed/license_delivery.html#check-whether-the-license-has-been-delivered)
