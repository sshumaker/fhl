---
layout: handbook-page-toc
title: Associating purchases with additional accounts
category: CustomersDot
description: Associating subscription with another account on CustomersDot account and for changing primary contact.
---

{:.no_toc}

----

Sometimes a customer may ask that a colleague be given the ability to manage a
subscription. This can be accomplished provided they also have a CustomersDot
account.

This process would also apply for requests to send a license to a different email
than the one used on the purchasing account.

#### Note about license recipient

Cloud activation codes can be sent to the `Sold To` contact only ([open issue](https://gitlab.com/gitlab-org/fulfillment-meta/-/issues/648)). You must [update the Zuora Sold To contact](#zuora-contact-change-workflow) before resending it.

## Ownership verification

First, we need **one** of the following in order to verify eligibility for the
ownership change:

1. Approval from the existing contact
1. Prior subscription contract
1. Recent GitLab invoice (last 12 months)
   - This option is not available for customers who purchased through a reseller. Instead, the reseller can either open a ticket with this request or the customer can CC the reseller and also confirm that they would like to authorize the reseller to participate in the ticket. The reseller can then provide the invoice as proof of identity.
1. Copy of last loaded license (Self-Managed only) in text format only.
   - Screenshots are not valid
   - To obtain the license code:
     - GitLab version 14.2 and newer: Use [license usage export](https://docs.gitlab.com/ee/subscriptions/self_managed/index.html#export-your-license-usage).
     - GitLab version 14.1, run the command `sudo gitlab-rails runner 'print License.current.data'` on the GitLab instance. N.B. this command can take a few minutes to complete.
     - GitLab versions older than 14.1, use `Download license` from the `Admin area > License` page.
   - License file can be decoded in customersDot from `Licenses` -> `Validate License` (`/admin/license/validate_license`)

**NOTE:** We do not accept vouches from GitLab Team Members (including Account Owners listed in SFDC) as proof of a customer's association to a subscription.

Please consider using the [Support::L&R::Change Customers Portal Contact](https://gitlab.com/gitlab-com/support/support-ops/zendesk-global/macros/-/blob/master/macros/active/Support/Self-Managed/Change%20Customers%20Portal%20Contact.yaml) macro to ask for this information. Be sure to copy the existing CustomersDot contact on the reply.

## Add subscription management contact workflow

If a customer requests to **add** another subscription management contact without removing the current contact,
first verify their identity as outlined under [ownership verification](#ownership-verification).

Once we have received one of the verification requirements, we can proceed to add a subscription management contact:

#### Important

Any time a CustomersDot customer is edited via the Admin, the Zuora account contact associated with the customer is updated. In case there is no Zuora contact with the same email, the Zuora account `Sold To` address is replaced. When adding additional subscription managers requires to edit the customer, it is important to press `save` on the original contact LAST, to ensure they remain the primary contact on their Zuora account.
Ensure alignment between the customer and the Zuora account:

1. Navigate to the provided Zuora account and check the value of `SSPChannel`. If it is marked as **Reseller**:
    1. Locate the customer to be added to the Zuora account
    1. Ensure the `Login activated` checkbox for the customer is **unchecked**. If the `Login activated` checkbox is checked:
       1. Go to the customer edit page.
       1. Uncheck the `Login activated` checkbox.
       1. Click `Save`.
       1. Locate the original `Sold To` contact in CustomersDot and click Save on the `Edit` page to ensure this contact remains the Sold To.

**Note:** Make sure you tell the customer that they cannot log in to the account because they purchased through a reseller.

Set the customer as a subscription management contact by creating a billing account membership:

1. Locate the CustomersDot billing account for the provided Zuora account
1. Navigate to the `Billing account memberships` section
1. Select the `+ Add new` action
1. Select the proper customer and CustomersDot billing account for the new subscription management request
1. Click `Save`

**Note:** If a customer already has a billing account membership, it is not currently possible to create a second billing account membership for this customer.

## Change subscription management contact workflow

This process should be a last resort for **non-reseller customers**, and [self-service options must first be explored](https://docs.gitlab.com/ee/subscriptions/#change-account-owner-information).

Reseller customers **do not** have access to CustomersDot -- for such customers, proceed to the [Support assisted option](#support-assisted-option) steps.

### Self-service option

**Ensure that the requestor has exhausted all self-service options:**

1. If the requestor is the existing Customers Portal account owner, inform them that
   to transfer account ownership they need to:
   1. [change the personal details](https://docs.gitlab.com/ee/subscriptions/#change-account-owner-information)
      to be the new account owner's personal details
   2. issue a
      [password reset](https://customers.gitlab.com/customers/password/new)
      to the new owner's email
   3. [link their GitLab account](https://docs.gitlab.com/ee/subscriptions/#change-the-linked-account)
      to ensure their subscription is kept in sync with the linked GitLab group
   4. Once the customer updates their account on Customers Portal, confirm that the Sold To contact in the
      Zuora account matches the Customers Portal account.
      Follow the [Zuora contact change workflow](#zuora-contact-change-workflow) to complete this update. [Note above](#note-about-license-recipient)
1. Otherwise, if they have access to the existing Customer Portal account owner's
   email address, guide them to:
   1. issue a [password reset](https://customers.gitlab.com/customers/password/new)
      to the existing owner's email
   2. [claim the account](https://docs.gitlab.com/ee/subscriptions/#change-account-owner-information)
      by changing over the personal details
   3. [link their GitLab account](https://docs.gitlab.com/ee/subscriptions/#change-the-linked-account)
      to ensure their subscription is kept in sync with the linked GitLab group
   4. Once the customer updates their account on Customers Portal, confirm that the Sold To contact in the
      Zuora account matches the Customers Portal account.
      Follow the [Zuora contact change workflow](#zuora-contact-change-workflow) to complete this update. [Note above](#note-about-license-recipient)

### Support assisted option

#### Important

- In order to change the subscription management contact, we should ask for the same [ownership verification](#ownership-verification) information.
- **Do not** change/move the zuora_account_id or salesforce_id of the customer account in CustomersDot.

Use this workflow if a customer requests to change a subscription contact by either taking over ownership,
handing over ownership, or re-gaining access to a subscription that was set-up by another person not in the
organization anymore.

We should try to always retain the original CustomersDot account with access to the Zuora subscription
until [Issue#4247](https://gitlab.com/gitlab-org/customers-gitlab-com/-/issues/4247) is resolved.

**Reason:**
Currently, an Order entry in the database is linked to one customer account only.
If the Order points at a Customer that doesn't have a `zuora_id` on it, the customer's Subscription cannot be found.
This may then lead to cloud activation errors and SaaS subscriptions not syncing to GitLab.com.

#### Reseller customer note

Please keep in mind that the customer (if purchased via a reseller) will only have one subscription contact in CustomersDot -
if such a customer is requesting multiple contacts be added, please recommend that they propose a shared inbox or email address for the account update.

#### Process

Only after ruling out the [self-service options](#self-service-option) above will we consider making
the requested ownership change:

1. Verify the customer's identity as outlined under [ownership verification](#ownership-verification).
1. If the customer has already created a new account and wants the ownership to be transferred.
    - Point them to [Issue#4247](https://gitlab.com/gitlab-org/customers-gitlab-com/-/issues/4247) and explain that might cause purchasing problems.
    - Change the email in the new account for example: `person@example.com` to `person_edited@example.com`
1. Update the `Name` and `Email` of the current account.
1. For SaaS only, use the [unlink GitLab.com Account mechanizer function](mechanizer.html#unlink-gitlabcom-account) if the accounts were linked
   - On the CustomersDot account, navigate to the `Show` tab and confirm there is a value under `Uid`.
   - The `Uid` is the ID of a GitLab account which can be checked via the Users API `https://gitlab.com/api/v4/users/<Uid>`
1. Trigger a [password reset](https://customers.gitlab.com/customers/password/new) to the new email, and for SaaS, to link their GitLab.com account.
1. Follow the [Zuora contact change workflow](#zuora-contact-change-workflow) to complete this update. [Note above](#note-about-license-recipient)

## Zuora contact change workflow

If a change is needed in the contact for future invoice and renewal related emails,
pass to Billing team by following the [Zuora Contact Change Workflow](https://about.gitlab.com/handbook/support/license-and-renewals/workflows/billing_contact_change_payments.html#zuora-contact-change).
