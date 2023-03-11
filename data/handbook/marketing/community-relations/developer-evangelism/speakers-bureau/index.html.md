---
layout: handbook-page-toc
title: "Join the Speakers Bureau"
description: "The Speakers Bureau is a group of GitLab team members and members of the wider GitLab community who are available to participate in events and deliver talks."
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## What is the Speakers Bureau?    

The Speakers Bureau is a group of GitLab team members and members of the wider GitLab community who are available to participate in events and deliver talks about GitLab, CI/CD, open source, remote work, and other topics. 

## Find a speaker  

A list of speakers bureau members can be found on our [Speakers Bureau page](/speakers/). After identifying a speaker for an event or other speaking opportunity, please [create an issue](https://gitlab.com/gitlab-com/www-gitlab-com/-/issues/new?issuable_template=speaker-request) to request the speaker. 

## Join the Speakers Bureau

If you would like to join the speakers bureau, we ask that you submit an MR to add yourself to the [Speakers Bureau page](/speakers/). This can be done by adding the following lines to the speakers.yml file in the www-gitlab-com project.

To create an MR for the Speakers Bureau page, you will need:

- Your personal Twitter / GitLab handles
- Links to recent (in the last 12 months) relevant presentations or talks you have delivered
- If you are not a GitLab team member, please include a link to video of a recent presentation.

Once you have the above items, follow these steps to add yourself to create your MR:

1. Go to the [speakers.yml file in the GitLab.com / www-gitlab-com](https://gitlab.com/gitlab-com/www-gitlab-com/blob/master/data/speakers.yml) project.
1. On the file page, click on the button labeled `Web IDE` near the middle of the page.
1. For community members: if prompted, click `Fork` to create a Fork of the repo which will allow you to make changes and submit a Merge Request.
1. You should see the `speakers.yml` file open in your browser. 
1. Copy and paste the entry below and enter your information into each of the blank fields.
```
# Example Entry
# - name: Ada Lovelace          # Your full name
#   region: North America       # One of North America, Central America, South America, Europe, Asia, Africa, Oceania
#   location: London, England   # What you want your location to be shown as
#   tagline: English mathematician and writer, chiefly known for inventing computer programming. # A quick 1 or 2 sentence description of your self and your speaking credentials.
#   twitter: olearycrew         # Your twitter handle
#   gitlab: brendan             # Your GitLab user name
#   affiliation: community      # One of teammember, heroes, or community
#   image: ada.png              # Place an image that is 344 × 201 into /source/images/speakers/
#   topics:                     # One or more of these topics
# #    - Remote Work
# #    - "Diversity, Inclusion, and Belonging"
# #    - CI/CD
# #    - Git
# #    - Security
# #    - DevOps
# #    - Open Source
# #    - Engineering
# #    - SRE / Operations
# #    - Kubernetes
# #    - Monitoring & Observability
# #    - UX Design
# #    - Documentation
# #    - Cloud Native
# #    - GitOps
#   presentations:              # A list of previous presentations for the back of the card
# #    - title: Foo
# #      link: https://
```
1. Once you have finished adding your information, click the `Commit` button in the bottom left. It should say something like `1 unstaged and 0 staged changes`. This will bring up a sidebar with an `Unstaged` and `Staged` area.
1. Check the file to ensure your updates are what you expect. If they are, click the check mark next to the filename to "stage" these changes.
1. Once you have verified all of the edits, enter a short commit message including what you've changed. Choose `Create a new branch`. Name the branch in the format of `YOURINITIALS-speakers-bureau` or similar. Tick the `Start a new merge request` checkbox. Then click `Commit` once more.
1. Click on the Activity link in the header to go to your Activity page. Once there, click on the blue `Create merge request` button at the top of the page.
1. Fill out the merge request details. Community members who are applying should tick the box to `Allow commits from members who can merge to target branch` as detailed on the [Allow collaboration on merge requests across forks](https://docs.gitlab.com/ee/user/project/merge_requests/allow_collaboration.html#enabling-commit-edits-from-upstream-members) page in our docs.
1. Add the `speakers-bureau` label and assign to `@johncoghlan`. Community members should mention `@abuango` in a comment in the merge request so our team can review and merge.

### Linting
When adding yourself to the Speakers Bureau, you may get a linting error in the build.  If that happens, ensure that the following requirements are met:

* Unique `name`: Your name must be unique - if you have the same name as another speaker add your middle inital or other identifiers 
* Unique `gitlab`: You must put your unique GitLab.com username in this field
* Unique `twitter`: You must put your unique Twitter username in this field
* Headshot: You must place your headshot in the `source/images/speakers` and reference it just by file name in the `picture` field.
* Valid `region`: Make sure your `region` field is one the allowed regions.  See [speakers_requirements.yml](https://gitlab.com/gitlab-com/www-gitlab-com/-/blob/master/data/speakers_requirements.yml#L1) for a list of the allowed regions.
* Valid `topics`:  Make sure your `topics` field only contains allowed topics.  See [speakers_requirements.yml](https://gitlab.com/gitlab-com/www-gitlab-com/-/blob/master/data/speakers_requirements.yml#L10) for a list of the allowed topics.

> To find the linters in the `www-gitlab-com` repository, search for the `lint:speakers_yml` namespace.

## Speaker Enablement

The Developer Evangelism team provides support to new and experienced speakers where necessary. These can range from presentation review, CFP ideation, or dry-run. [Learn more](/handbook/marketing/community-relations/developer-evangelism/speaker-enablement/) about the different resources and activities you can benefit from or drop a message on [Slack](https://gitlab.slack.com/archives/CMELFQS4B) if you need direct support. 

## Speaking at Events

For resources for GitLab team members who are planning on attending events or speaking at conferences, see [Speaker Resources](/handbook/marketing/corporate-communications/speaking-resources/). 

