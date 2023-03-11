---
layout: handbook-page-toc
title: "GitLab tiers"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

| Tier      | Delivery                  | License                   | Fee            |
| --------- | ------------------------- | ------------------------- | -------------- |
| Free      | self-managed and SaaS     | open source               | unpaid         |
| Premium   | self-managed and SaaS     | source-available          | paid           |
| Ultimate  | self-managed and SaaS     | source-available          | paid           |

## Definitions

1. Tier: a GitLab offering that provides a set of features at a particular price point.
1. Users: anyone who uses GitLab regardless of tier.
1. Customers: users on a paid tier.
1. Plans: the paid tiers only.
1. License: open source vs. source-available, for example moving a feature from a source-available tier to an open-source tier.
1. [Distribution](#history-of-ce-and-ee-distributions): self-managed CE vs. EE, for example you can have a EE distribution but in the Free tier.
1. Version: the [release of GitLab](/releases/), for example asking what version a user is on.

## Types of Users

1. Free User - anyone who uses GitLab free tier and does not pay for additional CI minutes or storage (but is eligible to beyond what is included in the free tier). 
2. Trial User - anyone who is currently in trial on one of the paid tiers.
3. Consumption User - anyone who uses GitLab free tier and pays by consumption for additional CI minutes or storage beyond what is included in the free tier.
4. Licensed User - anyone who is on a source-available license
    1. Ultimate User - a licensed user on Ultimate
    2. Premium User - a licensed user on Premium
    3. Starter User - a licensed user on Starter (No longer available, but some users are finishing out previously purchased licenses.) 
5. Program User - anyone who is on Premium or Ultimate tier through programs such as [GitLab for Startups](https://about.gitlab.com/solutions/startups/), [GitLab for Education](https://about.gitlab.com/solutions/education/) or [GitLab for Open Source](https://about.gitlab.com/solutions/open-source/)

## Delivery

In general each of the self-managed tiers match the features in the GitLab SaaS tiers. They have different names for two reasons:

1. There is not complete feature parity between self-managed and GitLab SaaS plans. For example, GitLab self-managed Premium, and Ultimate include [LDAP Group Sync](https://docs.gitlab.com/ee/administration/auth/ldap/index.html#group-sync) but GitLab SaaS Premium and Ultimate do not.
1. We want to know if a user is using self-managed or GitLab SaaS based on a just the tier name to prevent internal and external confusion.

When we need to specify which tier includes a particular feature using only one word (for example on our issue tracker), we reference the self-managed tiers by default because they tend to contain a superset of the GitLab SaaS tier features.
Where we can, we highlight both the self-managed and the GitLab SaaS tiers (like in [a release post](/releases/2018/02/22/gitlab-10-5-released/#instant-ssl-with-lets-encrypt-for-gitlab)).

## Libre, gratis, and free
When discussing their work, open source communities typically use the words "gratis" and "libre" instead of the word "free" to describe the nature of the software they create. This is because the English word "free" is an ambiguous word that can have several meanings: "no cost" ("free as in beer"), "with few or no restrictions" ("free as in speech"), or both. Open source communities therefore prefer to use the unambiguous term "gratis" when referring to "no cost" software and the term "libre" when refer to software "with few or no restrictions." Open source software is "libre" in that anyone is "free" to inspect, modify, and redistribute it. But open source software may or may not be "gratis."

Features that are part of GitLab's Free tier refer to open source software that is both gratis and libre—[free as in speech and as in beer](http://www.howtogeek.com/howto/31717/what-do-the-phrases-free-speech-vs.-free-beer-really-mean/). For more detail on this distinction, see [Wikipedia](https://en.wikipedia.org/wiki/Gratis_versus_libre).

## GitLab SaaS

We call the multi-tenant GitLab SaaS (with the G and L capitalized) since it is unambiguous and common.
We don't call it GitLab Cloud since most self-managed instances of GitLab are hosted in the cloud as well, and if we introduce single tenant instances it will be even more confusing.

## Personal vs group subscriptions
GitLab SaaS subscriptions are added to either a personal namespace or a group namespace. Personal subscriptions apply to a single user while Group subscriptions apply to all users in the Group.

## History of CE and EE distributions

Historically, GitLab was provided as two different software distributions, each with their own separate source code repository and documentation: [Community Edition (CE)](https://gitlab.com/gitlab-org/gitlab-ce/) and [Enterprise Edition (EE)](https://gitlab.com/gitlab-org/gitlab-ce/). As of GitLab version 12.3, released on 2020-09-22, [GitLab moved to a single code base](/blog/2019/08/23/a-single-codebase-for-gitlab-community-and-enterprise-edition/).

The "CE" and "EE" names referred to the actual software packages that were [downloaded and installed](/install/). Today, the single distribution is referred to as the "Official Linux package".

For a period of time, GitLab pricing tiers also used "CE" and "EE". When the [free, self-managed tier was changed from "CE" to "Free"](/blog/2018/04/20/gitlab-tiers/), it led to this dynamic:

**Free users** could use either one of two distributions: Community Edition (CE) and Enterprise Edition (EE). Enterprise Edition can be downloaded, installed, and run without a commercial subscription. In this case it runs using the open source license and only has access to the open source features. In effect, EE without a subscription, and CE, have the exact same functionality.

**Premium, and Ultimate users** could only use Enterprise Edition.

If a Free user was running CE and wanted to upgrade to a paid tier, they had to re-install and migrate to EE. The advantage of using EE as a Free user is that it is much easier to upgrade to a commercial subscription later on. All that's needed is to install a license key to access more features vs needing to re-install a different distribution. Today, GitLab's single distribution maintains these advantages.

See the [Tier Messaging](#tier-messaging) section for how to talk about GitLab, distributions, versions, tiers, pricing, and licenses.

### How we used the terms CE and EE

Community Edition (CE) and Enterprise Edition (EE) refer to software distributions of GitLab. We used to encourage customers to use the EE distribution since it provided the least painful upgrade path if/when users discovered they needed commercial features. If you aren't talking specifically about the distribution packages, then don't use these terms, [you are probably using them incorrectly](/handbook/communication/top-misused-terms/#enterprise_edition).

### Don't use CE/EE to refer to non-paid/paid **users**.

Users can be on the EE distribution for free. Distribution doesn't imply if a user is a customer or not.

    1. Say "users" when you mean all users - paid and unpaid.
    1. Say "customers" when you mean paid users.
    1. Say "Free users" when you mean unpaid users.

❌ Incorrect:  "Let's run a marketing campaign to encourage CE users to upgrade to a paid tier."

✅ Correct: "Let's run a marketing campaign to encourage Free users to upgrade to a paid tier."

### Don't use CE/EE to refer to **tiers**.

GitLab has 3 tiers: Free, Premium, and Ultimate. Distribution doesn't imply which tier a user is on.

    1. Say the "Free" when you mean the $0 tier.
    1. Say "Open source" when you mean features in the $0 tier.
    1. Say "Premium" or "Ultimate" to refer to those tiers.
    1. Optionally, say "GitLab Free," "GitLab Premium," or "GitLab Ultimate" when you want to refer to a pricing tier.
    1. Say "commercial tier" when you mean any paid tier.

❌ Incorrect:  "Let's move this feature to CE."

✅ Correct: "Let's open source this feature."

✅ Correct: "Let's move this feature from Ultimate to Free."

NOTE: Talking about "open sourcing a feature" is highly preferred to saying we want to "move a feature to Free." Open source calls attention to the fact that not only is the feature available for $0 now, it's also available for open community contribution in our MIT licensed codebase. "Free" only calls attention to the $0 price without highlighting our open source community.

## GitLab trials
We offer a [free trial for self-managed GitLab](/free-trial/#self-managed?glm_source=about.gitlab.com&glm_content=tiers) as well as a [free trial for GitLab SaaS Ultimate](https://gitlab.com/-/trial_registrations/new?glm_source=about.gitlab.com&glm_content=tiers).

### Why offer a free trial when we already have free tiers?

The trial allows users to have access to all of the features of GitLab Ultimate. Users on the Free plans (self-managed and SaaS) plans get access to a limited set of features for an unlimited amount of time. Trial users get access to a full set of features for a limited amount of time (30-days).

| License type | Features | Time Period |
| ------------ | -------- | ----------- |
| Free  | Limited (Open source features only) | unlimited |
| Trial        | Unlimited (access to all Ultimate features) | limited (30 days) |

## Open-source vs. source-available

GitLab is an open-core product that contains both open-source and source-available code.
The source-available code is proprietary (so not open-source) but you can view the source code.
Please don't use CE, EE, or Free to refer to the type of license since:

1. While most open source code is in GitLab CE, some code in EE is additional open source code since all our [javascript code is MIT licensed](https://about.gitlab.com/blog/2015/05/20/gitlab-gitorious-free-software/#free-javascript).
1. The majority of the code in EE is open source.
1. We might ship source-available code in Free that is free as in beer but not as in freedom (open source).

## Tier Messaging

When talking to customers, always use language that they are familiar with. They will likely not be familiar with terms we use internally as a company, it is important to use the customer’s language when you are talking to the customer to maximize understanding.

### Themes Hierarchy

The themes hierarchy is designed to communicate the value of GitLab **paid** features to customers.

1. **Value Drivers**: Themes roll into [customer value drivers](/handbook/sales/command-of-the-message/#customer-value-drivers). Value drivers describe what organizations are likely proactively looking for or needing and are top-of-mind customer topics that exist even if GitLab doesn’t. Value drivers may cause buyers to re-allocate discretionary funds, and they support a value-based customer conversation. Organizations adopt and implement GitLab for the following value drivers:
Value drivers are also highlighted within [tiers](https://about.gitlab.com/pricing/). 
1. **Themes**: Themes refer to sets of paid features. They highlight the benefits of features through grouping related paid features together, so customers can focus on a short-list of benefits rather than a long list of 80+ paid features. Themes can be found on [GitLab's pricing page](https://about.gitlab.com/pricing/). Each tier has about five themes. For example, better code reviews, compliance, or portfolio management. When clicking on a theme on the pricing page, users will find a list of paid features that relate directly to a specific theme. For example, better code reviews is a theme that encompasses the following paid features: code and productivity analytics, efficient merge request reviews, code quality reports, merge trains, and multiple approvers.
1. **Paid Features**: Paid features are small, discrete functionalities that are not included in GitLab's free tier. [Paid features](https://about.gitlab.com/features/by-paid-tier/) have historically been grouped into tiers, but this does little to call out key feature themes that differentiate one tier from the next and help customers to make sense of the key benefits derived from a long list of paid features. Paid features should be grouped into themes.

### Tiers and pricing messaging

1. Do always present Ultimate as _the_ product. Every customer and prospect would benefit greatly from the Ultimate product and it's the correct frame of reference to explain our complete vision.
1. Don't introduce lower tiers unnecessarily. We are consultative sellers with a high-value product. If a customer asks about pricing, the answer is "We have end-to-end DevOps in a single application ranging from our free offering up to Ultimate at $1,188 per user per year." Only go into detail on the lower tiers when appropriate based on your assessment of the customer's needs and progression in the product. Focus on the value sale as long as possible and only discuss tiers once there is a clear path forward to purchase.

### Use of “GitLab” by itself

1. Don't use the word "`GitLab`" alone unless you are referring to the company or an attribute that applies to both `GitLab Self-managed` and `GitLab SaaS`. If talking about an attribute that only applies to one delivery method but not the other, then specify (e.g. "GitLab SaaS does X" or "GitLab Self-managed does X").
1. Do specify `GitLab Self-managed` or `GitLab SaaS` when you are referencing something that is unique to that delivery method (e.g. a security bug that only affects GitLab SaaS).
1. Do use the word `GitLab` alone to refer to Ultimate. "GitLab does X" means, "GitLab Ultimate does X".
1. Don't use `GitLab` by itself when you really mean a specific, e.g. specify `GitLab Free` if you are referring to the free self-managed tier.

### Using open source, commercial, and source-available

Distinguish our $0 tiers from our paid tiers, by talking about our "open source" offerings and our "commercial" offerings.

For example, "I see that today you are using GitLab Free, I'd love to set up a call to discuss the value your business can get by upgrading from our open source offering to a commercial tier." (You could write the same sentence and use "paid" instead of "commercial" but that puts the focus on what they have to do, i.e. pay, instead of what they get, i.e. business-grade, commercial software.)

Use the terms "open source" and "source-available" to talk about our different license models.

**Don't** use CE and EE to refer to a specific code. `MIT Licensed` (code is open source) and `Proprietary` (code is source-available) refer to code. Both CE and EE distributions include MIT licensing.

### Using the word Enterprise

1. Do use "enterprise" to describe a market segment. e.g. good phrases to use are: "GitLab provides DevOps for the enterprise", "GitLab is enterprise-ready", "GitLab has many enterprise customers", and "GitLab provides enterprise software for the entire DevOps lifecycle."
1. Don't use "enterprise" as a modifier for tiers such as `Enterprise Starter`, `Enterprise Premium`, or `Enterprise Ultimate`.
1. Don't use the terms `Enterprise Edition Starter`, `Enterprise Edition Premium`, `Enterprise Edition Ultimate`, `EES`, `EEP`, or `EEU`. These have all been deprecated.

## GitLab FOSS

[GitLab FOSS](https://gitlab.com/gitlab-org/gitlab-foss/) is neither a tier, nor a distribution. It is a repository.
