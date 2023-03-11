---
layout: handbook-page-toc
title: "Community relations tools: Zapier"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

### Zapier subscription

We use Zapier to automate the task of forwarding mentions of GitLab, swag store orders, etc.

The Zapier subscription runs on the [Team plan](https://zapier.com/app/billing/plans), and is shared with the GitLab team.

### Zapier access

- URL: [https://zapier.com](https://zapier.com)
- Account: search for the shared Zapier account in 1Password's `Zapier` vault. Please file an [access request](/handbook/business-technology/team-member-enablement/onboarding-access-requests/access-requests/) if you cannot access that vault.

Once logged in, you can access, edit and create Zaps in the [Community Relations](https://zapier.com/app/zaps/folder/275996) folder

<i class="fas fa-hand-point-right" aria-hidden="true" style="color: rgb(138, 109, 59)
;"></i> After editing or creating a new Zap, remember to turn it on with the toggle switch next to the task's name on the Zap's list.
{: .alert .alert-warning}

### Current Zaps

List of Zaps that are enabled on the [Community Relations folder](https://zapier.com/app/zaps/folder/275996).

| Zap | Description | Involved Tools |
| --- | --- | --- |
| [about.gitlab.com + devops-tools comments](https://zapier.com/app/editor/47854205) | GitLab blog comments to `#mentions-of-gitlab` Slack channel, and DevOps Tools pages comments to Zendesk and `#devoptools-comments` Slack channel | Disqus, about.gitlab.com/blog, Slack | 
| [docs.gitlab.com comments](https://zapier.com/app/editor/47854205) | GitLab documentation comments to #docs-comments Slack channel. Monitored by the [Technical Writing](/handbook/product/ux/technical-writing/) team | Disqus, docs.gitlab.com, Slack |  
| [Community Relations MR Updates](https://zapier.com/app/editor/92097020) | All merged MRs with `Community Relations` label posted to #community-relations Slack channel | GitLab.com, Slack |  
| [GitLab Swag Store](https://zapier.com/app/editor/18836033) | GitLab store order to Printfection order | Printfection, Shopify |
| [Student Spotlights Application Alerts](https://zapier.com/app/editor/90643179) | Student Spotlights form submission notifications to `#student-spotlights-applications` Slack channel | Google forms/sheets, Slack | 
| [Post new Blogs to the GitLab forum](https://zapier.com/app/editor/148450001) | GitLab blog post is posted as [a new forum topic](/handbook/marketing/community-relations/workflows-tools/#gitlab-blog-forum-bot) | about.gitlab.com/blog, Discourse | 
| [Team member live on Twitch](https://zapier.com/app/editor/146185512) | New live stream posted to `#dev-evangelism-updates` | Twitch, Slack |
| [Hackernews: Slack notifications for front page mentions: GitLab](https://zapier.com/app/editor/58944326) | Hackernews: `GitLab` front page stories to `#developer-evangelism` Slack channel | HackerNews, Slack |
| [Hackernews: Slack notifications for front page mentions: Opstrace](https://zapier.com/app/editor/151511040) | Hackernews: `Opstrace` front page stories to `#developer-evangelism` Slack channel | HackerNews, Slack |
| [Hackernews: Slack notifications for front page mentions: Clickhouse](https://zapier.com/app/editor/153149325) | Hackernews: `Clickhouse` front page stories to `#developer-evangelism` Slack channel | HackerNews, Slack |
| [Hackernews: Slack notifications for front page mentions: Open Core](https://zapier.com/webintent/edit-zap/159764533) | Hackernews: `Open Core` front page stories to `#developer-evangelism` Slack channel | HackerNews, Slack |
| [Hackernews: Slack Notifications for mentions: GitLab](https://zapier.com/app/editor/52810208) | Hackernews: `GitLab` mentions to `#hn-mentions` Slack channel |  HackerNews, Slack |
| [Hackernews: Slack Notifications for mentions: DevOps Platform](https://zapier.com/app/editor/131452972) | Hackernews: `DevOps Platform` mentions to `#hn-mentions` Slack channel |  HackerNews, Slack |

#### Zaps for Hacker News

The Zaps poll the [Algolia search API for Hacker News](https://hn.algolia.com/api) and add specific URL parameters in order to 

- Query for a string in the posts; `?query="open%20core"`
- Filter by tags if the topic hit the front page of Hacker News: `&tags=front_page` 

Searching for a string with whitespaces requires to [use quotes](https://www.algolia.com/doc/api-reference/api-parameters/filters/#usage-notes) around the query parameter, for example `https://hn.algolia.com/api/v1/search?&query=%22open%20core%22&tags=front_page`. 

More API URL examples:

- Front page: https://hn.algolia.com/api/v1/search?&query=gitlab&tags=front_page
- Mentions: http://hn.algolia.com/api/v1/search_by_date?query="devops+platform"


#### gitlab-blog Forum Bot

The [`gitlab-blog`](https://forum.gitlab.com/u/gitlab-blog/summary) user is used to automatically post new [GitLab blogs](/blog/) as a new topic to the [Community](https://forum.gitlab.com/c/community/39) category.  This process is controlled through [Zapier](https://zapier.com/app/editor/148450001).  Zapier reads the blog RSS feed at `https://about.gitlab.com/atom.xml` and posts a new topic using the admin API key and `gitlab-blog` user for each new entry there.

The `gitlab-blog` credentials and admin API key are stored in the 1Password Marketing vault. Admins can directly edit the user in Discourse without login.
