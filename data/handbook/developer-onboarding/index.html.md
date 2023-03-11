---
layout: handbook-page-toc
title: "Developer Onboarding"
description: "Awesome! You're about to become a GitLab developer! Here you'll find everything you need to start developing."
---

Awesome! You're about to become a GitLab developer!
Make sure you've checked out our [handbook] beforehand, so you get a feeling
of how we work at GitLab. Below you'll find everything you need to start developing.
If something is missing, add it (as goes with everything at GitLab)!

### On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## GitLab Environments

We have multiple [GitLab environments](/handbook/engineering/infrastructure/environments/).

On those instances, please enable the
[performance bar](https://docs.gitlab.com/ee/administration/monitoring/performance/performance_bar.html)
by pressing <kbd>p</kbd> then <kbd>b</kbd> (even on production.)

Then, read how to use and enable the
[production Canary](/handbook/engineering/infrastructure/environments/canary-stage/)
on GitLab.com.

## Getting started with GitLab development

To start development, follow the instructions for the
[GitLab Development Kit](https://gitlab.com/gitlab-org/gitlab-development-kit).

## GitLab Repositories

GitLab consists of many subprojects. A curated list of GitLab Repositories
can be found at the [GitLab Engineering Projects](/handbook/engineering/projects/) page.

Almost all repositories are available on both GitLab.com and dev.gitlab.org. We
also mirror to dev.gitlab.org for availability reasons and [GitHub](https://github.com/gitlabhq)
for historical reasons.

All issues should be filed on GitLab.com.

## Infrastructure

For everything related to infrastructure, check out the
[Infrastructure handbook](/handbook/engineering/infrastructure/).
In particular [production architecture](/handbook/engineering/infrastructure/production/architecture/) might be useful for onboarding.

If you need a VPS for any reason, it's probably easiest to set one up at DigitalOcean. Ask another developer for access.

## Basics of GitLab development

### Workflow

Please see the [engineering workflow document][eng-wf] in the handbook and read
the [developer documentation][dev-doc].

[eng-wf]: /handbook/engineering/workflow/
[dev-doc]: https://docs.gitlab.com/ee/development/

### Security

Read the [developer security documentation][sec-doc] prior to working on a security issue.

[sec-doc]: https://gitlab.com/gitlab-org/release/docs/blob/master/general/security/developer.md

### Quality

One of GitLab's strengths is its high quality of software. To achieve this we've
introduced some requirements to all source code that is contributed. All
requirements are mentioned in [the Contribution guide][contrib-guide].
Make sure you read and follow it.

### Dependencies

GitLab can be installed through an Omnibus package or from source on different
Linux distributions and macOS. In order to maintain portability, we need to
avoid adding extra dependencies and use of exotic database extensions. Every
time you choose between changes in the application code or adding new
dependencies, you should give priority to the first because this is easier to
maintain and set up. If you still need to bring new dependencies to GitLab, ask
another developer or the CTO for advice.

### Submit your code

In GitLab all code should go through a review process before it can be merged.
Make sure you submit a merge request for any changes you've made.
When the merge request is ready, it should be assigned to [someone else on the team](/handbook/engineering/workflow/code-review/).
This person is then responsible for reviewing your code and merging it.
Optionally, you can request another developer to help or review by writing a comment.
If a merge request is not assigned, it will probably be ignored and create
unnecessary delays.

Don't work on one task for multiple days before submitting a merge request.
Even the biggest task can be split into smaller tasks.
Try to submit a merge request for each part of the functionality.
This means that we expect multiple merge requests per week from you.
Smaller merge requests are more likely to receive good feedback and will get
merged sooner.

Unless the change is very minor, or is fixing a bug that was introduced in the
same version, create a changelog entry using the
[`Changelog` Git commit trailer][changelog-entry].
Do not include your name in the entry as we only do that to give recognition to
volunteer contributors.

[changelog-entry]: https://docs.gitlab.com/ee/development/changelog.html

### Working on GitLab EE (developer licenses)

GitLab EE requires a license key to be used.

Team members should [open an issue](https://gitlab.com/gitlab-com/team-member-epics/access-requests/-/issues/new?issuable_template=GitLab_Team_Member_License_request)
using the `GitLab_Team_Member_License_request` template. In the issue, request for a license that is valid for a year, and provide "Developer on-boarding"
as the reason for a longer expiration.

Wider community members should contact the [Code Contributor Program](https://about.gitlab.com/handbook/marketing/community-relations/code-contributor-program/#contact)
who should use the [GitLab Support Internal Request](https://gitlab-com.gitlab.io/support/internal-requests-form/) (**Other > Wider Community License**) to request a license.

[Learn more about working with licensing and subscriptions internally.](https://about.gitlab.com/handbook/support/internal-support/)

### Ruby Gems

When publishing gems for GitLab, you should:

1. Ensure the gem doesn't become orphaned, or unable to be published, by either:
   - Using the [`gitlab-qa`](https://rubygems.org/profiles/gitlab-qa) RubyGems.org user.
     The user credentials can be found in the 1password `Engineering` vault.
   - Adding it to the list of [Gem Owners](https://guides.rubygems.org/managing-owners-using-ui) on RubyGems.org. You can also do this from a command line with the `gem` tool. For example, run this command to make the `gitlab-qa` user a co-owner:

      ```shell
      $ gem owner <gem_name> --add gitlab-qa
      ```

1. Follow the [gem development documents](https://docs.gitlab.com/ee/development/gemfile.html#gitlab-created-gems).
1. Optional. Add some or all of the following users as co-owners:
   - [Marin Jankovski](https://rubygems.org/profiles/marinjankovski)
   - [Rémy Coutable](https://rubygems.org/profiles/rymai)
   - [Stan Hu](https://rubygems.org/profiles/stanhu)
1. Optional. Add any other relevant developers as co-owners.

#### New version release

Gem projects should use the [shared CI/CD config](https://gitlab.com/gitlab-org/quality/pipeline-common/-/blob/master/ci/gem-release.yml)
to release and publish new gem versions by adding the following to their `.gitlab-ci.yml`:

```yaml
include:
  - project: 'gitlab-org/quality/pipeline-common'
    file: '/ci/gem-release.yml'
```

Note that this will include access token configuration inherited from the `gitlab-org` group, which will
be used to upload the gem package to rubygems.org.

Make sure to create a `v0.0.0` tag if you don't already have any [SemVer](https://semver.org) tag so
that the auto-release can compute the diff when releasing the actual first version of the gem.
This job will handle building and publishing the gem, as well as creating the tag, release and populating its release notes by
using the [Generate changelog data](https://docs.gitlab.com/ee/api/repositories.html#generate-changelog-data) API endpoint.

For instructions for when and how to generate a changelog entry file, see the dedicated [Changelog entries](https://docs.gitlab.com/ee/development/changelog.html) page.

[To be consistent with the GitLab project](https://docs.gitlab.com/ee/development/changelog.html),
Gem projects could also define a changelog YAML configuration file at `.gitlab/changelog_config.yml` with the same content
as [in the `gitlab-styles` gem](https://gitlab.com/gitlab-org/ruby/gems/gitlab-styles/-/blob/master/.gitlab/changelog_config.yml).

To ease the release process, you could also create a `.gitlab/merge_request_templates/Release.md` MR template with the same content
as [in the `gitlab-styles` gem](https://gitlab.com/gitlab-org/ruby/gems/gitlab-styles/-/raw/master/.gitlab/merge_request_templates/Release.md)
(make sure to replace `gitlab-styles` with the actual gem name).

## Relevant links

- [Engineering Handbook](/handbook/engineering/)
- [Engineering Workflow](/handbook/engineering/workflow/)
- [Product Handbook](/handbook/product/)

[handbook]: /handbook
[in the open]: /2015/08/03/almost-everything-we-do-is-now-open/
[contrib-guide]: https://about.gitlab.com/community/contribute/
