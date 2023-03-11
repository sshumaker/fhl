---
layout: handbook-page-toc
title: Service Desk Single-Engineer Group
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Service Desk Single-Engineer Group

The Service Desk SEG is a [Single-Engineer Group](/company/team/structure/#single-engineer-groups) within our [Incubation Engineering Department](/handbook/engineering/incubation/).

### Vision

Our goal is to provide a complete, yet lightweight and customizable customer support solution that seamlessly integrates with the GitLab ecosystem and brings customers, support staff and developers closer together.

### Mission

- Make Service Desk useful for professional support teams so they efficiently and effectively work through their support issues.
- Helping organizations build a professional and on-brand customer support workflow that grows with the business.
- Making Service Desk an integral part of the GitLab support workflow by providing the tools our teams need.
- Helping managers and support ops automate repetitive tasks for their support staff.
- Increase awareness of the capabilities of GitLab Service Desk and how it can help our customers handle customer support.

### Recent updates and showcases

Please feel free to [subscribe to this GitLab issue to receive notifications](https://gitlab.com/gitlab-org/incubation-engineering/service-desk/meta/-/issues/3) when new updates are available.

#### Monthly showcases

**Watch the latest showcase video**

<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/rw-2fqtUodQ" frameborder="0" allowfullscreen="true"> </iframe>
</figure>

| Date | Video |
| ---- | ----- |
| [January 2023](https://gitlab.com/gitlab-org/incubation-engineering/service-desk/meta/-/issues/7) | [Update Video](https://www.youtube.com/watch?v=rw-2fqtUodQ){:target="_blank"} |

#### Update videos

**Watch the latest update video**

<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/CiP7LRqm8vo" frameborder="0" allowfullscreen="true"> </iframe>
</figure>

| Update / Date         | Summary                                                                                                                                               | Video                                                                          |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| Update 3 (2023-01-20) | [Foundation &amp; verification](https://gitlab.com/gitlab-org/incubation-engineering/service-desk/meta/-/issues/7)                          | [Update Video](https://www.youtube.com/watch?v=CiP7LRqm8vo){:target="_blank"}  |
| Update 2 (2023-01-06) | [First MR &amp; upcoming tasks breakdown](https://gitlab.com/gitlab-org/incubation-engineering/service-desk/meta/-/issues/6)                          | [Update Video](https://www.youtube.com/watch?v=jbUX611DR-g){:target="_blank"}  |
| Update 1 (2022-12-09) | [Product Vision &amp; customizable E-Mail Addresses](https://gitlab.com/gitlab-org/incubation-engineering/service-desk/meta/-/issues/4)               | [Update Video](https://www.youtube.com/watch?v=AmKy4IGmevc){:target="_blank"}  |

We are also [exploring ideas, existing issues and user feedback](https://gitlab.com/gitlab-org/incubation-engineering/service-desk/meta/-/issues/2). Please feel free to contribute.

### Current focus

#### Customizable e-mail address on a per-project basis

Right now GitLab does not support a fully customized and professional e-mail experience throughout the 
communication with the customer. You can add e-mail forwarding from your own e-mail address to the Service Desk 
intake e-mail address, but the sender of the inquiry will always receive answers from the default GitLab 
instance address. That is especially a show-stopper for gitlab.com customers as they do not want to have 
GitLab e-mail addresses in their customer communication.

We are actively working on [bringing configurable e-mail addresses on a per-project basis to GitLab Service Desk](https://gitlab.com/gitlab-org/gitlab/-/issues/329990).
The [proposed solution](https://gitlab.com/gitlab-org/gitlab/-/issues/329990#note_1192437371) will involve little changes to existing 
functionality and we will iterate on that to make it even easier to use in the future.

Customers will need to configure e-mail forwarding from their desired Service Desk e-mail address to the 
provided Service Desk intake e-mail address by the GitLab instance. They will then add SMTP credentials for that address so
the GitLab instance will be able to send e-mails on behalf of that configured e-mail address. 
We will also allow `Reply-To` e-mail headers to use the configured e-mail address to deliver a complete package.

If you have questions or would like to share feedback, see [this issue](https://gitlab.com/gitlab-org/gitlab/-/issues/329990).

#### Obfuscate email addresses of Service Desk issues based on user role

Making sure private data is protected no matter where a Service Desk issue ends up. If you do not have at least the reporter role in a GitLab project or group, you won’t be able to view the email address of the author of a Service Desk issue and issue email participants in general. No matter whether it’s a public or private project or the issue is confidential or not.

**This will ship in GitLab 15.9**

If you want to get more into the details, [check out the merge request which also links to all related issues](https://gitlab.com/gitlab-org/gitlab/-/merge_requests/108901).

### Background

We have a [Service Desk offering](https://about.gitlab.com/direction/plan/certify/#service-desk) in GitLab that we'd like to make an integral part of the GitLab support workflow.  We have early usage, and a community of prolific contributors, however internally this work has been deprioritized. and this is a great opportunity for the Incubation Engineering department to make the next stage of development that meets customer needs.

### Product Development Group affinity

- [Certify group in Plan stage](https://about.gitlab.com/handbook/product/categories/#certify-group) owns Service Desk right now, but [it will move to Monitor Stage](https://gitlab.com/gitlab-com/Product/-/issues/5171)
- [Respond group in Monitor stage](https://about.gitlab.com/handbook/product/categories/#respond-group) will be the new home for Service Desk (see above) long term.
- [Project management group in Plan stage](https://about.gitlab.com/handbook/product/categories/#project-management-group) as Service Desk issues use all of GitLabs planning functionality
