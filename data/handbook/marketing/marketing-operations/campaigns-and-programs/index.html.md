---
layout: handbook-page-toc
title: "Campaigns and Programs"
description: "Campaigns are used to track efforts of marketing tactics - field events, webcasts, content downloads."
---
## On this page
{:.no_toc .hidden-md .hidden-lg}
- TOC
{:toc .hidden-md .hidden-lg}


## Campaigns

Campaigns are used to track efforts of marketing tactics - field events, webcasts, content downloads. The campaign types align with how marketing tracks spend and align the way records are tracked across three of our core systems (Marketo, Salesforce and Bizible) for consistent tracking. Leveraging campaign aligns our efforts across Marketing, Sales and Finance.

### Campaign Large Buckets
Campaign buckets are used to improve reporting at a high level and Allocadia forecasting. A bucket must be selected when a new campaign is created.

|Name|Description|Examples|
|-------|--------------|---------|
|Brand          | Activities meant to elevant the GitLab brand          | All-Remote, share of voice campaigns        |
|Lead Generation|Efforts designed to bring in NEW leads to our database|Inbound Marketing, Conferences, Content Syndication, Webinars, Prospect Events in regions|
|Pipeline Generation & Acceleration|Efforts to develop and accelerate leads in our database to purchase|Webinars, Workshops, Owned Events|
|Users & Community| Campaigns geared towards GitLab users and Community|Commit, Meetups|
|E-Commerce Conversion|Campaigns that do not require a touch by sales to close|`Buy Now` in our store|

Campaign Types and Large Buckets will not always be 1:1, as certain programs could fall into multiple buckets (like webcasts, content).

### Campaign Cost Tracking

For information on how Marketing tracks campaign costs, please visit [this page](/handbook/marketing/#how-marketing-tracks-campaign-expenses).

### Campaign Type & Progression Status

A record can only progress **one-way** through a set of event statuses. A record _cannot_ move backward though the statuses.

i.e. Record is put into `Registered` cannot be moved backwards to `Waitlisted`


#### Conference

Any event  that we have paid to sponsor, have a booth/presence and are sending representatives from GitLab (example: AWS re:Invent, DevOps Enterprise Summit). This also includes any virtual event that we sponsor and/or participate in that we do not own the registration but will generate a list of attendees, engagement.

In a virtual conference, GitLab will pay a sponsorship fee to receive a virtual booth and sometimes a speaking session slot or panel presence. Presence of a virtual booth is a requirement due to success criteria. [Read more](/handbook/marketing/virtual-events/external-virtual-events/#virtual-conferences).

For list loads greater than 5,000 `attendees`, Mktgops will need to confer with the `Field Marketing Director` on legitimacy of labeling the program members as `success` as doing so affects `Bizible Touchpoints`. Follow [directions here](/handbook/marketing/marketing-operations/campaigns-and-programs/#instructions-how-to-update-conferences-with-more-than-5000-attendees) on how to do this (MktgOps only).

**Bizible:** This is tracked as an _offline_ channel, because we do not host a registration page, and receive a list of booth visitors post-event. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Sales Invited | Invitation/Information about event sent by Sales/SDR |  |
| Sales Nominated | Sales indicated record to receive triggered event email sent by Marketing |  |
| Marketing Invited | Marketing geo-targeted email |  |
| Waitlisted| Holding state if registration is full will be moved to Registered if space opens| |
| Registered | Registered for event||
| No Show | Registered but no verification of attendance, presumed no show | |
| Meeting Requested | Meeting set to occur at conference |  |
| Meeting No Show | Scheduled meeting at conference was cancelled or not attended |  |
| Meeting Attended | Scheduled meeting at conference was attended | Yes |
| Attended| Attended the event| Yes |
| Visited Booth | Stopped by booth for any reason | Yes |
| Follow Up Requested | Requested to be followed up with by sales post event | Yes |
| Attended On-Demand | Watched/consumed conference materials post-event on-demand | Yes| 

#### Content Syndication

White Paper or other content offer that is hosted by a third party.

**Bizible:** This is tracked as an _offline_ channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Downloaded | Downloaded content | Yes |

#### Direct Mail

This is when a package or piece of mail is sent out.

**Bizible:** This is tracked as an _offline_ channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success | E-gift Card or Physical Gift |
| ------------- | ---------- | ------- | ------------ |
| No Action | Default starting position for all records |  | Not applicable |
| Sales Nominated | Sales indicated record to receive triggered event email sent by Marketing |  | Not applicable |
| Processed | Physical gift shipping request is being processed  |  | Physical |
| Sent | Email with e-gift card has been sent to recipient |  | E-gift card |
| Opened | The prospect has opened the Reachdesk offer emailed to them |  | E-gift card |
| Claimed | The recipient has claimed the Reachdesk gift | Yes | E-gift card |
| Clicked | The prospect has clicked the link in the offer emailed to them |  | E-gift card |
| Shipped | The recipient's gift has been shipped |  | Physical |
| Delivered | The selected gift has been successfully delivered to the recipient | Yes | Physical |
| Cancelled | The recipient has requested their gift be cancelled |  | Physical |
| Returned | The recipient has returned their gift |  | Returned |


#### Executive Roundtables

This is used for campaigns that can either be organised through a 3rd party vendor or GitLab, covering both in-person and virtual roundtables. It is a gathering of high level CxO attendees run as an open discussion between the moderator/host, GitLab expert and delegates. There usually aren't any presentations, but instead a discussion where anyone can chime in to speak. The host would prepare questions to lead discussion topics and go around the room asking delegates questions to answer. [Read More](/handbook/marketing/virtual-events/external-virtual-events/#overview).

**Bizible:** This is tracked as an _offline_ channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Sales Nominated | Sales indicated record to receive triggered event email sent by Marketing |  |
| Waitlist | Holding state if registration is full will be moved to `Registered` if space opens |  |
| Registered | Registered for the event |  |
| No Show | Registered, but did not attend the event |  |
| Attended | Attended the Event | Yes |
| Follow Up Requested | Requested follow up during the event | Yes |

#### Gated Content

White Paper or other content offer.

**Bizible:** This is tracked as an _online_ channel. 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Downloaded | Downloaded content | Yes |

#### Inbound - offline

**Bizible:** This is tracked as an _offline_ channel because touchpoints cannot be applied directly via online means, e.g. Drift and PQL handraises. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Requested Support | Took a handraise action to request support from the GitLab team ||
| Requested Contact | Filled out Contact, Professional Services, Demo or Pricing Request | Yes |

#### Inbound Request 

Any type of inbound request that requires follow up.

**Bizible:** This is tracked as an _online_ channel.  

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Requested Support | Took a handraise action to request support from the GitLab team ||
| Requested Contact | Filled out Contact, Professional Services, Demo or Pricing Request | Yes |

#### Operational

This is used for non-traditional list uploads in which we are looking to a) avoid scoring the uploaded leads b) avoid tradition nurture emails c) fulfill some other various operational related task. e.g., educational conference list uploads.

**Bizible:** This is tracked as an _online_ channel because we participated in an event, where applicable.

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| Member | default starting position for all records |  |
| Registered | Registered (presumably did not attend) |  |
| Attended | Attended live event |  Yes |
| Attended Virtually | Attended an event virtually. Attendance can be live or post-event | Yes |

#### Owned Event

This is an event that we have created, own registration and arrange speaker/venue (example: GitLab Commit or Meetups). Also considered in this grouping would be 3rd party auxiliary events that are added on to a conference sponsorship (i.e a happy hour or VIP dinner at a conference).  

**Bizible:** This is tracked as an _online_ and as an _offline_ channel because we manage the registration process through our website. Whenever someone registers, a TP will be created based on that online activity while another  TP is added based on the campaign sync rules, for the campaign members with success statuses. 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Subscribed to Updates | Subcribed to GitLab event updates via form fill |  |
| Sales Invited | Invitation/Information about event sent by Sales/SDR |  |
| Sales Nominated | Sales indicated record to receive triggered event email sent by Marketing |  |
| Marketing Invited | Marketing geo-targeted email |  |
| Waitlisted | Holding state if registration is full will be moved to `Registered` if space opens |  |
| Registered | Registered for event |  |
| Cancelled | Registered, but cancelled ahead of the event |  |
| No Show | Registered but did not attend event |  |
| Attended | Attended event live| Yes |
| Attended On-demand| Watched/consumed the presentation materials post-event on-demand| Yes |
| Follow Up Requested | Requested additional details about GitLab to be sent post event | Yes |

#### Paid Social

**Bizible:** This program is designated to house leads and programs brought in by social related campaigns (e.g. Linkedin campaigns) and is tracked as an _offline_ channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Responded | Took an action related to social campaigns, like a form fill  | Yes |

#### Partner - MDF

This is for an activity that our partner is executing utilizing MDF Funds. We track membership, but the partner, not GitLab follows up with these leads. See more details [here](/handbook/marketing/channel-marketing/partner-campaigns/#mdf-funded-campaigns).

**Bizible:** This is tracked as an _offline_ channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| Member | default starting position for all records |  |
| Sales Nominated | status for when leads have been sales nominated for the program |  |
| Responded | Attended event or campaign |Yes|

#### Prospecting

This program type is specific to non-event related list uploads, such as partner lists or data upload centric lists. 

**Bizible:** This is not tracked on Bizible.

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Uploaded | Status lead is normally transitioned to upon successful upload |  |
| Do Not Use (Responded) | Not to be used. Included because Marketo requires a `success` step  | Yes  |
| Member | Indicative of a special member status for this program type. Meaning of "special" is dependent on use case |  |


#### Self-Service Virtual Event

This is a light weight virtual event that can be hosted on GitLabber's personal zoom.

**Bizible:** This is tracked as an _online_ channel if registrants come through a marketo form, otherwise it will be an _offline_ channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Sales Nominated | Status for when Sales and Marketing want to extend an event invitation | |
| Waitlisted | Holding state if registration is full will be moved to `Registered` if space opens |  |
| Registered | Registered for event |  |
| No Show | Registered but did not attend event |  |
| Attended | Attended event | Yes |
| Attended On-demand | Watched/consumed the presentation materials post-event on-demand | Yes |
| Follow Up Requested | Requested follow up during the event | Yes | 

#### Speaking Session

This campaign type can be part of a larger Field/Conference/Owned event but we track engagement interactions independently from the larger event to measure impact. It is something we can drive registration. It is for tracking attendance at our speaking engagements.

**Bizible:** This is tracked as an _offline_ channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Sales Invited | Invitation/Information about event sent by Sales/SDR |  |
| Sales Nominated | Sales indicated record to receive triggered event email sent by Marketing |  |
| Marketing Invited | Marketing geo-targeted email |  |
| Registered | Registered or indicated attendance at the session |  |
| No Show | Registered but did not attend event |  |
| Attended | Attended speaking session event | Yes |
| Follow Up Requested | Had conversation with speaker or requested to be followed up with by sales post event | Yes |

#### Sponsored Webcast

This is webcast hosted on an external partner/vendor platform. The status of `Attended On-demand` accounts for GitLab hosted On-Demand and non-GitLab hosted On-demand webcasts. [Read more](/handbook/marketing/virtual-events/external-virtual-events/#overview).

**Bizible:** This is tracked as an _online_ channel if registrants come through a marketo form, otherwise it will be an _offline_ channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Sales Nominated | Used by marketing for invitee tracking | | 
| Registered | Registered for webcast |  |
| No Show| Registered but did not attend event |  |
| Attended | Attended event | Yes |
| Follow Up Requested | Requested to be followed up with from GitLab | Yes |
| Attended On-demand | Watched/consumed the presentation materials post-event on-demand | Yes |

#### Survey

A survey that we or a 3rd party sends out. Tracks respondents and new leads we receive. 

**Bizible:** This is tracked as an _offline_ Bizible channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| Member | default starting position for all records |  |
| Sales Nominated | Sales indicated record to receive triggered event email sent by Marketing |  |
| Invited | Was invited, but did not participate in survey |  |
| Filled-out Survey | Filled out survey | Yes |
| Follow Up Requested | Filled out survey and requested to be contacted by sales | Yes |

#### Trial

Track cohort of Trials for each product line (Self-managed or SaaS) to see their influence.

**Bizible:** In-product self-managed and SaaS trials are tracked as an **offline** Bizible touchpoint. The self-managed trial utilizing a Marketo form is an **online** Bizible touchpoint.

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Signed Up | Signed up for Trial | Yes |

#### Vendor Arranged Meetings

Used for campaigns where a third party vendor is organizing one-to-one meetings with prospect or customer accounts. This does not organize meetings set internally by GitLab team members. An example would be a "speed dating" style meeting setup where a vendor organized meetings with prospects of interest to GitLab. [Read more](/handbook/marketing/virtual-events/external-virtual-events/#overview).

**Bizible:** This is tracked as an _offline_ Bizible channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Registered | Registered for the event |  |
| No Show | Registered, but did not attend the event |  |
| Attended | Attended the Event | Yes |
| Follow Up Requested | Had conversation with speaker or requested additional details to be sent post event | Yes |

#### Webcast

Any webcast that is hosted and held by GitLab. There are a few different groups that run webcasts. Go their specific pages to see additional details on setup.
- [Campaign webcasts](https://about.gitlab.com/handbook/marketing/virtual-events/webcasts/#campaign-webcasts)
- [Field Marketing webcasts](https://about.gitlab.com/handbook/marketing/field-marketing/field-marketing-owned-virtual-events/#webcasts-1)
- [Partner webcasts](https://about.gitlab.com/handbook/marketing/virtual-events/webcasts/#partner-webcasts)
- [On24 webcasts](/handbook/marketing/marketing-operations/on24)

**Bizible:** This is tracked as an _online_ Bizible channel as well as an _offline_ channel. We own the registration process so whenever a person registers to a webcast, a TP will be created based on the Bizible snippet that lives on our landing pages, while another TP is created for campaign members with success/responded statuses. 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Sales Invited | Invitation/Information about event sent by Sales/SDR |  |
| Sales Nominated | Sales indicated record to receive triggered event email sent by Marketing |  |
| Marketing Invited | Marketing geo-targeted email |  |
| Registered | Registered through online form |  |
| No Show | Registered, but did not attend live webcast |  |
| Attended | Attended the live webcast | Yes |
| Follow Up Requested | Requested to be followed up with by sales post event | Yes |
| Attended On-demand | Watched the recorded webcast | Yes |

#### Workshop

An in-person or virtual workshop where the attendees are guided through an agenda of real life use cases within GitLab.

For logistical setup and more information, go [here](https://about.gitlab.com/handbook/marketing/field-marketing/field-marketing-owned-virtual-events/#virtual-workshops-1).
**Bizible:** This is tracked as an _offline_ Bizible channel. Touchpoints for offline channels are created through our AMM (formerly known as Bizible) campaign sync rules that can be found in this [spreadsheet](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564). 

| Member Status | Definition | Success |
| ------------- | ---------- | ------- |
| No Action | default starting position for all records |  |
| Sales Invited | Invitation/Information about event sent by Sales/SDR |  |
| Sales Nominated | Sales indicated record to receive triggered event email sent by Marketing |  |
| Marketing Invited | Marketing geo-targeted email |  |
| Waitlisted | Holding state if registration is full will be moved to Registered if space opens |  |
| Registered | Registered or indicated attendance at the session |  |
| Cancelled | Registered, but cancelled ahead of the event |  |
| No Show | Registered, but did not attend event |  |
| Attended | Attended workshop event | Yes |
| Follow Up Requested | Requested additional details about GitLab to be sent post event | Yes |

# Marketo Program and Salesforce Campaign set-up

The Marketo programs for the corresponding campaign types have been prebuilt to include all the possible necessary smart campaigns, email programs, reminder emails and tokens that are to be leveraged in the building of the program.

For **Linkedin Social Ads** follow the instructions documented in [the Linkedin section](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-setup-linkedin-lead-gen-form-gated-content-only)

For **virtual events**, there are additional set up details on this [page](/handbook/marketing/virtual-events).

For all other campaign types, follows steps below. All steps are required.   

## Parent/Child Campaigns  

For some tactics, there are mutiple campaigns that occur as a part of a single initiative. Some examples of these could be a conference with speaking session, direct mail, content syndication, or hybrid events (where in-person and virtual leads will be tracked separately). When this happens, a `parent` campaign should be created in SFDC and have each `child` campaign represent the individual tactics. The parent SFDC campaign should not include any members, or include bizible touchpoints. Additionaly, if you are an Allocadia user, you will not include a sub-category ID in Marketo when syncing to SFDC and creating the new parent campaign. Since we do not have the same parent/child relationship structure available in Marketo, you will create a folder that will house all of the shared tactics together. 

To assocate a child SFDC campaign to a parent SFDC campaign, go into what will be the child SFDC campaign and at the top of the campaign, click `Edit`. This will open the SFDC fields and then you can add the parent SFDC campaign name into the `Parent` field. Click `Save`.

An example of a folder setup in Marketo is:
- Conference Name (Folder)
   - Conference Name (Program w/ members)
   - Direct Mail Name (Program w/ members)
   - Speaking Session 1 (Program w/ members)
   - Speaking Session 2 (Program w/ members)

## Important Notes
1. The `Active` checkbox must be checked on the SFDC campaign for Marketo to be able to "see" the campaign. This will happen automatically if you follow the process below, but if there is a time you cannot find a SFDC campaign in Marketo, check to make sure that box is checked in SFDC. Additionally, if this box is unchecked, Marketo cannot send leads or update campaign member status for that SFDC campaign.
1. If you are creating a parent campaign, please make sure that the campaign name of a parent campaign reflects the fact that it's a parent, by adding `_Parent` at the end of the Campaign Name. In the event of a mishap, when a parent campaign was setup by mistake to house responded campaign members,  adding `_Parent` at the end of the campaign name, makes sure that it gets seen by our campaign sync rules that [control the generation of touchpoints for offline campaigns](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564) and does not create double touchpoints for campaign members that may be housed in both the parent and child campaigns. 
1. If you are creating a campaign that relies on offline touchpoint generation, please make sure to double check that the campaign type is selected appropriately and that the campaign name does not contain words like `test`, `DONTUSE`, `template`, `parent`, because based on the [campaign sync rules that govern the creation of offline touchpoints](https://docs.google.com/spreadsheets/d/1xR2Q7YKskfNaxclnfGOkK8Vi739zdKypQ6GgF9MLG58/edit#gid=92970564), these campaigns will not have touchpoints created for them. 
1. We have a trigger in SFDC that stamps the start date, end date, reporting date, and fiscal quarter by taking the first 8 characters of the name of the campaign (if they are numbers) and converting that into a date (example: 20210505 == 5/5/2021, so YYYYMMDD). So, campaigns starting with a number must contain a valid date, otherwise you will receive an error.
1. Campaign statuses other than `Aborted` are automatically set by SFDC workflow based on Start and End Dates.

|Status|Definition|When does it update?|
|------|--------|--------|
|Planned|The campaign is expected and has been set up, but the start date hasn't happened yet (could also be where its pulled back to if an event is postponed)|Prior to the Campaign Start date - upon Creation|
|In Progress|The campaign has begun |On Start date|
|Aborted|Campaign has been suspended, cancelled, aborted|Manually when campaign is aborted|
|Completed|The campaign took place and has ended|After the Campaign End Date|

## Steps to Setup Marketo programs and Salesforce Campaigns

### Step 1: Clone the Marketo program indicated below

Be advised that some templates are being used for both `in-person` and `virutal events`. These templates have been marked as `Hybrid template`. For these templates, the naming convention is slightly different in that additional campaign information appears in the name. When naming the program, `EventType` is replaced with either `Virtual`, `In-Person`, or `Hybrid` (if an event will be both in-person and virtual).  

If this is to set up a program that involves a channel partner, you must also follow the directions on that [setup page](/handbook/marketing/channel-marketing/partner-campaigns/#joint-marketing-campaign-set-up). You will still clone the program from the list below to get started.

#### How to Clone the Marketo program

- Click on the appropriate template for your tactic below (you must be logged into Marketo to proceed)
- Right click on the template in Marketo and select `Clone`
- In the `Clone To` field, select `A campaign folder`
- In the `Name` field, input the campaign name (this should be the campaign name previously created in Allocadia - example: 20220704_BestEventEver)  - The date should be the START date of your campaign. 
- In the `Folder` field, select the appropriate folder based on your campaign type. Most folders are also organized by fiscal year and quarter.
- In the `Description` field, paste your epic URL
- Click `Create`

##### Hybrid Marketo Templates


- Executive Roundtables - `Hybrid template`: [YYYYMMDD_ExecutiveRoundtable_Topic_Region_EventType_template](https://app-ab13.marketo.com/#ME6028A1)
- Speaking Session - `Hybrid template`: [YYYYMMDD_SpeakingSession_EventType_Template](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/ME5092A1)
- Vendor Arranged Meetings (1:1 meetings) - `Hybrid template`: [YYYYMMDD_ArrangedMeetingsVendorName_Region_EventType_template](https://app-ab13.marketo.com/#PG5698A1)
- GitLab Hosted Workshops - `Hybrid template`:   
[For virtual workshops, please follow directions in the virtual workshop set-up section.](/handbook/marketing/field-marketing/field-marketing-owned-virtual-events/#virtual-workshop-logistical-set-up) In-person workshops utilize a similar setup, but do not involve the Zoom requirements. If you have a workshop to set up that is not one of the workshops listed below, you can still utilize any of these templates for backend setup and then use a [copy dock](https://docs.google.com/document/d/1j43mf7Lsq2AXoNwiygGAr_laiFzmokNCfMHi7KNLjuA/edit#heading=h.tl82wncgutxu) to indicate all copy adjustments that are required (you will also update the baseline Marketo tokens during the setup process).
   - Project Management: [YYYYMMDD_Workshop_ProjectManagement_EventType](https://app-ab13.marketo.com/#ME6536A1)
   - Security: [YYYYMMDD_Workshop_SecurityWorkshop_EventType](https://app-ab13.marketo.com/#ME6521A1)
   - DevOps Automation: [YYYYMMDD_Workshop_DevOpsAutomation_EventType](https://app-ab13.marketo.com/#ME6532A1)
   - Advanced CI/CD: [YYYYMMDD_Workshop_CI/CD_EventType](https://app-ab13.marketo.com/#ME6807A1)  
   - Jenkins [YYYYMMDD_Workshop_Jenkins_EventType](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/ME8285A1) 

##### Other Tactic Marketo Templates
- Conference - `Virtual`: [YYYYMMDD_YYYYMMDD_Vendor_VirtualConfName1 (Virtual Conference Template)](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/ME7624A1)
- Conference - `In person`: [skip to specific setup details here](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-setup-in-person-conferences)
- Content Syndicaton: [skip to specific setup details here](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-setup-content-syndication-in-marketo-and-sfdc)
- Direct Mail: [YYYYMMDD_DirectMail_Template](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG5392A1)
    - Direct Mail not needing a Marketo Program: [skip to specific setup detais here](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-setup-direct-mail-campaigns)
- Gated Content: [YYYY_Type_Content_Template](https://app-ab13.marketo.com/#PG5111A1)
- Integrated Campaign: [FY20IntegratedCampaign_Template](https://app-ab13.marketo.com/#PG4924A1) 
- Surveys - For templates and setup instructions for surveys (both general surveys and SimplyDirect surveys) skip to specific setup details [here](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-setup-surveys-in-marketo-and-sfdc).
- Owned Event - `In-person`: [YYYYMMDD_OwnedEvent_EventType_Template](https://app-ab13.marketo.com/#ME4722A1)
- Owned Event - `Virtual - Hopin only`: [YYYYMMDD_OwnedEvent_Hopin_EventType_Template](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/ME11445A1) 
    - For Events using HopIn, follow all steps below in addition to steps outlined [here](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-use-hopin-connector). 

##### Webcasts and Self-Service Marketo Templates
- BrightTALK GitLab Hosted Webcast: [YYYYMMDD_WebcastTopic_Region](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/ME6946A1)
- WebEx GitLab Hosted Webcast: [YYYYMMDD_WebEx_WebcastTopic_Region](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/ME8983D4)
- Zoom GitLab Hosted Webcast: [YYYYMMDD_WebcastTopic_Region](https://app-ab13.marketo.com/#ME5512A1)
- Self-Service Virtual Event without Promotion: [YYYYMMDD_SelfServiceTopic_Region](https://app-ab13.marketo.com/#ME5143A1)
- Self-Service Virtual Event with Promotion (with or without Marketo Landing Page): [YYYYMMDD_SelfServiceTopic_Region (with Promotion)](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/ME8760A1)
- Sponsored Webcast: [YYYYMMDD_ExternalWebcastVendorName_Topic_Region](https://app-ab13.marketo.com/#PG5523A1)

#### Partner Campaign Setup
- Partner MDF Funded campaigns go [this page](/handbook/marketing/channel-marketing/partner-campaigns/#mdf-funded-campaigns).
- Joint GitLab/Partner campaigns, follow the directions for each campaign type above/below. There are additional steps [here](/handbook/marketing/channel-marketing/partner-campaigns/#joint-marketing-campaign-set-up) you'll need to complete as well.
- Partner Trials setup, go to [this page](/handbook/marketing/channel-marketing/partner-campaigns/#trial-campaign-set-up)

### Step 2: Sync to Salesforce

- At the program main screen in Marketo, where it says `Salesforce Sync` "not set", click on "not set"
    - Click "Create New." The program will automatically populate the campaign tag, so you do not need to edit anything.
    - If you are a user of Allocadia, you will need to add the Allocadia sub-category ID to the `Description` field. 
    - Click "Save"

### Step 3: Update Marketo tokens

- Complete the information for each token. Instructions for what to enter for each token are included in the template.
    - Note that it is important that all tokens are completed as the "Interesting Moments" Smart Campaigns pushes information to Salesforce based on the tokens. Depending on the campaign, some auto-responders and emails rely on tokens as well.
    - Note that the token for `Event Location` should be filled in with the `City` for `In-Person` events and `Virtually` for `virtual events`.
    - You do not need to update the following tokens upon setup:
        - ((my.email header image url}} - This is optional. You will need this if you had custom images created.
        - {{my.ondemandurl}} - This will be entered AFTER the event date. It is the link to the recorded webcast. You will need to come back after the event and update this token.
- Update the utm_campaign field following the process outlined [here](https://about.gitlab.com/handbook/marketing/utm-strategy/#utm-campaign). 
- **Partner Campaigns** will need to also to update the `{{my.partner name}}` and `{{my.partner crm id}}` for proper routing 
- For live events, be sure to update the `reply email` token. This is used in the confirmation email. You need to add the correct email address for cancellations or special accomodations, and update the subject to something descriptive. Keep the `%20` between each word in the subject so the subject populates correctly.

### Step 4a: Activate Marketo smart campaign(s)
* If this is a `Vendor Arranged Meeting` skip this step. The campaign and interesting moments will be run as a batch campaign after the list is loaded. 
* If this is `Self-Service with Promotion` or `Speaking Session` follow the below activation instructions:
     * Click the `Smart Campaigns` folder
     * Select the `01a Registration Flow` smart campaign
     * The correct program should automatically apply when cloned, so *you don't need to do anything here.* However, you can confirm that the campaign tag appears on in the Smart List and Flow. If the name of the template appears anywhere, replace it with the campaign tag.
     * Click to the `Schedule` tab and click `Activate`     
     * (NO ACTION) If a list is used to import registrants/attendants, the `03 - Processing - No Shows / Attendees` smart campaign will be run after the list is uploaded.
     * For `Speaking Session` also select the `02-Interesting Moments` smart campaign, click to the `Schedule` tab and click `Activate` 
* If this is an `Executive Roundtable`
     * Click on the `Campaigns` folder
     * Click on `Interesting Moments`, click to the `Schedule` tab and click `Activate`    
     * If you are creating a Marketo landing page for this event, click on `01 Registration Flow`, click to the `Schedule` tab and click `Activate`. If you are doing a list upload, this step is not necessary.
* If this is `Workshop` follow the below activation instructions:
     * Click the `Smart Campaigns` folder
     * Select the `00 Interesting Moment` smart campaign, navigate to the Schedule tab and select `Activate`
     * Select the `01a Registration Flow` smart campaign for virtual webinars or the `03 In-person Processing` smart campaign for in-person events
     * The correct program should automatically apply when cloned, so *you don't need to do anything here.* However, you can confirm that the campaign tag appears on in the Smart List and Flow. If the name of the template appears anywhere, replace it with the campaign tag. 
     * Click to the `Schedule` tab and click `Activate` 
* If this is an `Owned Event` (not Hopin) follow the below activation instructions:
     * Click the `Campaigns` folder
     * If you have a Marketo registration page for this event, select the `01b - Registration` smart campaign
     * The correct program should automatically apply when cloned, so *you don't need to do anything here.* However, you can confirm that the campaign tag appears on in the Smart List and Flow. If the name of the template appears anywhere, replace it with the campaign tag.
     * Click to the `Schedule` tab and click `Activate`      
     * Select the `02a - Interesting Moments` smart campaign
     * The correct program should automatically apply when cloned, so *you don't need to do anything here.* However, you can confirm that the campaign tag appears on in the Smart List and Flow. If the name of the template appears anywhere, replace it with the campaign tag.
     * Click to the `Schedule` tab and click `Activate`  
     * LIST UPLOAD ONLY: If you do not have a registration page and responses will be uploaded via a list load, MOps will activate the `02b - Manual Upload Processing` campaign if necessary.
* If this is an `Owned Event` (Hopin), follow the `Update the Salesforce campaign` instructions in Step 5, then follow the activation instructions [here](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-use-hopin-connector)).
* For all other campaign types, follow the below activation instructions:
     * Click the "Smart Campaigns" folder
     * Select the `Interesting Moments` smart campaign. 
     * The correct program should automatically apply when cloned, so *you don't need to do anything here.* However, you can confirm that the campaign tag appears on in the Smart List and Flow. If the name of the template appears anywhere, replace it with the campaign tag.
     * Click to the "Schedule" tab and click `Activate`.
     * Select the `01 Processing` smart campaign. (Does not apply to Virtual Conference or External Webcast)
     * The correct program should automatically apply when cloned, so *you don't need to do anything here.* However, you can confirm that the campaign tag appears on in the Smart List and Flow. If the name of the template appears anywhere, replace it with the campaign tag.
     * Click to the "Schedule" tab and click `Activate`.

      
- If you do not see an `Interesting Moments` campaign, check to see if that step is in `01 Processing` or `Viewed on Demand` campaigns.
- For `Speaking Sessions` with pre-registration, find the `Pre-Registration` folder, and activate the `01 - Form Fill` step after populating the smart list with the correct form and landing page.

### Step 4b: Setting Landing Page / Smart Campaign Expiration (Asset Expiration)
As of early 2022, Adobe has introduced a new feature to Marketo called `asset expiration`, which can be read about in Marketo's documentation [here](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/local-asset-expiration.html?lang=en#:~:text=Right%2Dclick%20on%20your%20desired,Choose%20an%20expiration%20date). This applies to smart campaigns and landing pages. For GitLab's use case, we have enabled this feature for the following role permissions: `Field Marketing User`, `Marketing Program Managers` and `Marketing User`. If you do not have these permissions would like this feature enabled, please submit an `access request`. 

##### Asset Expiration Use Cases 
All programs have different necessities so it will be important to determine how `asset expiration` should be utilized for various program types. Guidance can be supplied by MktgOps, if needed, but utilize this method for the majority of cases: 
- `Conference`, `Direct Mail`, `Executive Roundtable`, `Owned Event`, `Self-Service Virtual Event` (if no on-demand component), `Speaking Session`, `Sponsored Webcast` (if no on-demand component), `Survey`, `Vendor Arranged Meeting`, `Workshop`: For one-time programs that are completely done after a specific date and will not use an `Attended On-Demand` member status over time, set the expiration of assets at 4 weeks after the event and at the end of the day, so at 23:55 PST. For example, if a `conference` or `executive roundtable` program type occurs on the April 3, schedule asset expiration for end day on May 1.
- `Content syndication` or Campaigns where the end of the campaign is difficult to pinpoint: there are 2 different options to consider: 
    - Set up expiration **12 weeks after the estimated campaign end**, again at the end of the day. This is useful for campaigns where a third-party is handling lead collection for us and we are manually uploading lead lists. This also supplies a buffer in the event the SLA is not met on schedule and the campaign runs longer than anticipated. 
    - **Do not use asset expiration at all**. We often have content syndication focused programs that go on indefinitely so expiration does not make sense to utilize in this case. Assets can be discontinued in the future.
- `Gated Content`: It is not recommended to use asset expiration as these remain in use for long periods of time. 
- `Webcast`: It is not recommended to use asset expiration as these typically have an on-demand component.

##### Setting Asset Expiration On A Program
- Right click the Marketo program to open the program menu and select `Set local asset expiration`. Please note, this will not work without the correct permissions.
- A menu with all expiration capable assets will be shown as a segmented list. Example assets that can appear are `landing pages`, `active trigger campaigns` and `Reocurring batch campaigns`. 
- Use the asset checkboxes to select all assets you wish to set an expiration for and select `set expiration` when ready. Assets that should be expired are `landing pages`, `active trigger campaigns` and `Reocurring batch campaigns`. Set your date and time and then submit. 
  - Prioritize setting expirations on  `smart campaigns`.
  - Be mindful of which smart campaigns are set to expire and when because such an event will disable program `registation` and `on-demand` flows.
- To remove expirations at a later date, right click on the program to return to the capable assets and submit changes. 


### Step 5: Update the Salesforce campaign
*If you are utilizing the Allocadia, please see below instructions.*  

- Now go to Salesforce.com and check the [All Campaigns by create date](https://gitlab.my.salesforce.com/701?fcf=00B4M000004oVF9) view. Sort by create date and your campaign should appear at the top. You may also search for your campaign tag in the search box. Select the campaign.
    - Change the `Campaign owner` to your name
    - Update `Large Bucket` based on [criteria above](/handbook/marketing/marketing-operations/campaigns-and-programs/#campaign-large-buckets)
    - Confirm that start date and end date populated correctly (this is automated).
    - Update the `Is this an in person event` dropdown, based on `in-person` vs `virtual` type
    - Update the event epic
    - Update the description (if any)
    - Update `Budgeted Cost` - If cost is $0 list `1` in the `Budgeted Cost` field. - NOTE there needs to be at least a 1 value here for ROI calculations, otherwise, when you divide the pipeline by `0` you will always get `0` as the pipe2spend calculation.
    - Update `Region` and `Sub-region`, if these are local or targeted to a specific region
    - Update `Budget Holder` -  Do keep in mind that the `Budget Holder` field should be updated **only if**:
        -  the campaign results in offline Bizible touchpoints based on campaign type (i.e. content syndication, sponsored webcast, etc.) - **NOTE:** an offline Bizible touchpoint happens when we gather a lead offline and in order for the system to have this name you must go through a [list upload process](/handbook/marketing/marketing-operations/list-import/);     
**OR:**
        -  there were Gitlab Dollars spent on the campaign (Field, Digital, Corporate, Community etc.) - can be left blank in the cases when we have campaigns that do not utilize budget; - **NOTE:** By updating the budget holder, we do **NOT** run the risk of double counting touchpoints, however, do keep in mind that since the field is not always filled out, it shouldn't be used for measuring each team's performance.   
    - All other fields on the campaign are not required and are not used for reporting - take `Status` as an example. You WOULD update this field to `Aborted` if the campaign was cancelled for any reason. We have a process that goes into more detail specifically when [offline events are cancelled](/handbook/marketing/events/#cancellation-of-offline-events). 
    - Click "Save"
- Add the Marketo program link and SFDC campaign link to the epic.
- For all SFDC campaign types run by Corporate Events or Field Marketing, please check the `High Priority` check box on the campaign level, as this is part of a [pilot we are running in FY23 Q3 & Q4](https://gitlab.com/gitlab-com/marketing/marketing-operations/-/issues/6905) with the business development team.

### Step 5: Update the Salesforce campaign - Using Allocadia 
Using an integration from Allocadia > Marketo, Marketo > SFDC, the information you've provided in Allocadia will push to your SFDC campaign.  

**Please Note:** You must NOT edit the campaign until the Allocadia connector has time to work. This is normally done near-real time, but if the data does not push immediately, be aware it can take minutes to hours to do so. You'll know the Allocadia connect has completed its work when you see the SFDC campaign owner change from Marketo Integration to the name of the actual person who is running the camapign as well as well as when all details are populated from Allocadia to SFDC. If you edit the campaign before the connector pushes the data over, it will break the build and you will manually have to edit all of the fields listed. For additional Allocadia details [go here](/handbook/marketing/strategy-performance/allocadia/#salesforcecom-sfdc).    

#### Training Videos for Setting up SFDC Campaign - Using Allocadia

* [Instructional Video](https://youtu.be/1681EBw5344)
* [Sync Results Video](https://youtu.be/PocOPnJY4w0)

Based on the [Step 5. list above](/handbook/marketing/marketing-operations/campaigns-and-programs/#step-5-update-the-salesforce-campaign), the only thing you will need to manually update in SFDC is the following: 
    - `Budgeted Cost` in SFDC pulls from your `plan` number, not your `forecast` number from Allocadia. If you do not have a `plan` cost in Allocadia then Budgeted Cost in SFDC will remain blank. If this is the case, you will want to add in your Budgeted Cost manually into your SFDC campaign. The initial Plan Cost in the campaign needs 1 night to synch. The campaign meta data is a one time synch, where as the Actual Cost in Campaign (which is run off of the Campaign Tag to be Created field in Allocadia), synchs every nightly. **Please Note:** `Budgeted Cost` in SFDC pulls from your plan number, not your forecast number from Allocadia. If you do not have a plan cost in Allocadia then `Budgeted Cost` in SFDC will remain blank. If this is the case, you will want to add in your `Budgeted Cost` manually into your SFDC campaign. If cost is $0 list `$1` in the `Budgeted Cost` field. There needs to be at least a $1 value here for ROI calculations, otherwise, when you divide the pipeline by `0` you will always get `0` as the pipe2spend calculation.

### Waitlist processing - Owned Event, Workshop, Webcasts
If you need to change an event from registration to waitlist, or you want to start off with a waitlist, use these instructions.
- Confirm that the email copy you would like to use is set-up in the `Confirm - Waitlist` email. This email uses tokens and should be set for you, but you can customize as necessary.
- Confirm that the {{my.event owner email address}} is completed in the tokens section. The Waitlist program will send an alert to this email address so you know each time someone is added to the waiting list based on this token.
- Deactivate the `01b Registration` Smart Campaign
- Activate the `01a Waitlist` Smart Campaign
- Activate the `01c Waitlist to Registered` Smart Campaign
You have now activated the waiting list processing. If you need to reactivate Registration, you will deactivate the two Waitlist campaigns, and reactivate `01b Registration`. 

### Moving from Waitlist to Registered - Owned Event, Workshop, Webcasts
Use these instructions to move people from the waiting list to Registered.
- Click on the Marketo program (the name of the campaign)
- Click on `Members`
- Change the filter to `Waitlisted`
- Click on the person/people you would like to move to Registered. They will highlight when they are selected.
- Click on `Change Status`
- Select `Registered`
Once you click `Registered`, the status will change and the `01c Waitlist to Registered` Smart Campaign will send the Registration Confirmation email.


## Steps to Setup in-person Conferences

### Step 1: [Clone this program](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/ME12196A1)

- Use format `YYYYMMDD_Conference_EventType`

### Step 2: Sync to Salesforce

- At the program main screen in Marketo, where it says `Salesforce Sync` with "not set", click on "not set"
    - Click "Create New." The program will automatically populate the campaign tag, so you do not need to edit anything.
    - If you are a user of Allocadia, you will need to add the Allocadia ID sub-category ID to the `Description` field. 
    - Click "Save"

### Step 3: Update Marketo tokens

- Update all tokens as they feed the email and interesting moments
   - You do not need to update `Request` tokens if there are no meetings being set up for the conference
   - If you are scheduling in person meetings, be sure to update the `reply email` token. This is used in the confirmation email. You need to add the correct email address for cancellations or special accomodations, and update the subject to something descriptive. Keep the `%20` between each word in the subject so the subject populates correctly.

### Step 4: Activate Marketo smart campaign
- `00 Send Sales-Driven Invite` (optional) can be turned on and scheduled to send on a reoccuring basis if sales and XDRs are going to be inviting people to the conference. This is not required on all campaigns, and Verticurl will activate after building the Sales-Driven email. After scheduling, Sales can add someone to the campaign in SFDC and that person will be automatically sent an email invite. There is a separate email for sales invites listed in the `email` folder
- `01 Manual upload processing` this will be activated by MOps if a manual upload is required. If you upload using the self-service process, this is not required.
- `02 Add as Marketing Invited` should only be used if XDRs are planning to follow up and drive attendance to the event. This should be scheduled AFTER the first email invite is scheduled to send. It will update everyone who had the email invite sent to them as `Marketing Invited`. They will be updated in the campaign and visible in SFDC. **Do not use this unless there is planned event drivers**
- `03 Interesting Moments` Activate this campaign. This should be turned on before any lists are uploaded.

### Step 4a. Meeting Request Processing
These steps are not yet configured. If you are planning to do this for your next event, please create an issue with the Marketing Operations team.

### Step 4b. Set-up Asset Expiration
- Right click the Marketo program to open the program menu and select `Set local asset expiration`. Please note, this will not work without the correct permissions.
- A menu with all expiration capable assets will be shown as a segmented list. Example assets that can appear are `landing pages`, `active trigger campaigns` and `Reocurring batch campaigns`. 
- Use the asset checkboxes to select all assets you wish to set an expiration for and select `set expiration` when ready. Assets that should be expired are `landing pages`, `active trigger campaigns` and `Reocurring batch campaigns`. Set your date and time and then submit. 
  - Prioritize setting expirations on  `smart campaigns`.
  - Be mindful of which smart campaigns are set to expire and when because such an event will disable program registation flows.
- To remove expirations at a later date, right click on the program to return to the capable assets and submit changes. 

### Step 5: Update the Salesforce campaign

- Now go to Salesforce.com and check the [All Campaigns by create date](https://gitlab.my.salesforce.com/701?fcf=00B4M000004oVF9) view. Sort by create date and your campaign should appear at the top. You may also search for your campaign tag in the search box. Select the campaign.
    - Change the `Campaign Owner` to your name
    - Update `Large Bucket` based on [criteria above](/handbook/marketing/marketing-operations/campaigns-and-programs/#campaign-large-buckets)
    - Update the event epic
    - Update the description
    - Update `Start Date` to the date of launch
    - Update `End Date`
    - Update `Budgeted Cost` - If cost is $0 list `1` in the `Budgeted Cost` field. - NOTE there needs to be at least a 1 value here for ROI calculations, otherwise, when you divide the pipeline by `0` you will always get `0` as the pipe2spend calculation.
    - Update `Region` and `Subregion` if you have the data available
    - Click Save
- Add the Marketo program link and SFDC campaign link to the epic.
- If the program is being ran by Digital Marketing, add the SFDC campaign under the parent campaign `Demand Gen Pulishers/Sponsorships`  

**If utilizing Allocadia, follow these [steps](/handbook/marketing/marketing-operations/campaigns-and-programs/#step-5-update-the-salesforce-campaign---using-allocadia).**  

## Steps to Setup Content Syndication in Marketo and SFDC

### Step 1: [Clone this program](https://app-ab13.marketo.com/#PG5149A1)

- Use format `YYYY_Vendor_NameofAsset`
- If the content syndication is part of a package with an external vendor, promoting several assets or webcasts, keep all of the Marketo programs together in a folder for easy access as part of a single vendor program.

### Step 2: Sync to Salesforce

- At the program main screen in Marketo, where it says `Salesforce Sync` with "not set", click on "not set"
    - Click "Create New." The program will automatically populate the campaign tag, so you do not need to edit anything.
    - If you are a user of Allocadia, you will need to add the Allocadia ID sub-category ID to the `Description` field. 
    - Click "Save"

### Step 3: Update Marketo tokens

- Change the `Content Title` to be the title as it appears in the Content Syndication program
     - If you have multiple assets, you can add additional tokens by dragging the text token into the main window and naming it (for example Content Title2)  
- Change the `Content Type` to be the type of content
    - The only available options are `Whitepaper`, `eBook`, `Report`, `Video`, or `General`
    - If you add a Content Type value other than the above, the record will hit an error when syncing to Salesforce because these are the only currently available picklist items for `Initial Source`
  

### Step 4: Activate Marketo smart campaign


- `02 Interesting Moments` If you have multiple assets, you can create different interesting moments to indicate which asset was downloaded. To do this, click on Flow. In step 1 (Interesting Moment), click Add Choice. Choice 1 will appear. Select If `Last Event Notes` contains [name of asset]. Then, Type: Milestone, Description: Enter the Interesting Moment that you would like to appear. You can do this for as many assets as you have. Activate this campaign. This should be turned on before any lists are uploaded. 
- Click to the "Schedule" tab and click `Activate`. It should be set that a person can only run through the flow once.
    - IMPORTANT: When you do your list upload, you must use the exact same wording in the `Last Event Notes` field so the automation will trigger. For example, you can say `Downloaded Guide to Software Supply Chain Security" in the Last Events Notes field. In Marketo, you can use `software supply chain` in the choice and the correct Description will trigger. Do not use the same string of words in your choices. You can see an example of the Interesting Moments set-up in the flow of [program](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/SC21549C3ZN19). Disregard the rest of the processing as our process has changed.
- `01 Manual upload processing` - this will be activated by MOps if it is required. It will only be used on a manual upload and is not necessary if you use the self-service upload process.
    - When the leads are loaded to the campaign, the leads will immediately have an interesting moment, +15 score, and initial source, person source and person status update as needed.

### Step 4a: Set-up Asset Expiration
- `Content syndication` or Campaigns where the end of the campaign is difficult to pinpoint: there are 2 different options to consider: 
    - Set up expiration **12 weeks after the estimated campaign end**, again at the end of the day. This is useful for campaigns where a third-party is handling lead collection for us and we are manually uploading lead lists. This also supplies a buffer in the event the SLA is not met on schedule and the campaign runs longer than anticipated. 
    - **Do not use asset expiration at all**. We often have content syndication focused programs that go on indefinitely so expiration does not make sense to utilize in this case. Assets can be discontinued in the future.

##### Setting Asset Expiration On A Program
- Right click the Marketo program to open the program menu and select `Set local asset expiration`. Please note, this will not work without the correct permissions.
- A menu with all expiration capable assets will be shown as a segmented list. Example assets that can appear are `landing pages`, `active trigger campaigns` and `Reocurring batch campaigns`. 
- Use the asset checkboxes to select all assets you wish to set an expiration for and select `set expiration` when ready. Assets that should be expired are `active trigger campaigns` and `Reocurring batch campaigns`. Set your date and time and then submit. 
  - Prioritize setting expirations on  `smart campaigns`.
  - Be mindful of which smart campaigns are set to expire and when because such an event will disable program registation flows.
- To remove expirations at a later date, right click on the program to return to the capable assets and submit changes. 

### Step 5: Update the Salesforce campaign

- Now go to Salesforce.com and check the [All Campaigns by create date](https://gitlab.my.salesforce.com/701?fcf=00B4M000004oVF9) view. Sort by create date and your campaign should appear at the top. You may also search for your campaign tag in the search box. Select the campaign.
    - Change the `Campaign Owner` to your name
    - Update `Large Bucket` based on [criteria above](/handbook/marketing/marketing-operations/campaigns-and-programs/#campaign-large-buckets)
    - Update the event epic
    - Update the description
    - Update `Start Date` to the date of launch
    - Update `End Date`
    - Update `Budgeted Cost` - If cost is $0 list `1` in the `Budgeted Cost` field. - NOTE there needs to be at least a 1 value here for ROI calculations, otherwise, when you divide the pipeline by `0` you will always get `0` as the pipe2spend calculation.
    - Update `Region` and `Subregion` if you have the data available
    - Click Save
- Add the Marketo program link and SFDC campaign link to the epic.
- If the program is being ran by Digital Marketing, add the SFDC campaign under the parent campaign `Demand Gen Pulishers/Sponsorships`  

**If utilizing Allocadia, follow these [steps](/handbook/marketing/marketing-operations/campaigns-and-programs/#step-5-update-the-salesforce-campaign---using-allocadia).**  

## Steps to Setup Surveys in Marketo and SFDC
There are two templates to consider when setting up surveys in Marketo, one being specific to Simply Direct and the other a more general survey template. For this section and where instructions diverge, Simply Direct instructions will be labeled with `a` and the more general set up with `b`. 

Simply Direct will provide you with an unique `Survey Name` that they will pass over into Marketo via the API populating the `Person Source` and the `SurveyName` fields. This name is unique to each survey that is ran. `Person Source` will not update if the lead already exists in Marketo.

SimplyDirect is also passing over the survey Q&A through the `Comment Capture` field. This will populate via a URL on the Interesting Moment and the `Web Form` field, so that the SDR following up will have full access to all of the survey questions and answers.

**Please Note: Once you have created your survey program, please ping Marketing Ops in the `#mktops` Slack channel and link your program for review. Each survey is unique and may require tweaks to the setup.**

### Step 1: Clone program template
- a. [Simply Direct template](https://app-ab13.marketo.com/#PG6164A1)
- b. [General survey template](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG6402A1)
- Use format `YYYY_MM_SurveyName`

### Step 2: Sync to Salesforce

- At the program main screen in Marketo, where it says `Salesforce Sync` with "not set", click on "not set"
    - Click "Create New." The program will automatically populate the campaign tag, so you do not need to edit anything.
    - If you are a user of Allocadia, you will need to add the Allocadia ID sub-category ID to the `Description` field. 
    - Click "Save"

### Step 3a: Update SurveyName across Smart Lists, Flows and Tokens
- Contact SimplyDirect and ask for the SurveyName they will pass to Marketo
- Click into `01 Processing`
     - In Smart List, change every `SurveyName` to the name you were given. There are 3 fields on the smartlist you must change. Tokens will not work, you must update in the smart list. Do not include any extra spaces!
     - In the Flow, on step 1 `Change Data Value` update `SurveyName` to the name you were given.
     - Click to the "Schedule" tab and click `Activate`. It should be set that a person can only run through the flow once.
- BEFORE launch of the survey, have SimplyDirect send an existing lead, and a new lead through to make sure both are being captured.
- Fill in necessary program tokens.

### Step 3b: Create issue for lead upload (if not Simply Direct)
- If the survey requires a manual upload via a list upload, focus attention on updating the `01 Processing` batch smart campaign. For manual list uploads, the batch will be activated manually by MktgOps during the upload process. 
- If the survey requires a Zapier automation, consult MktgOps [via issue](https://gitlab.com/gitlab-com/marketing/marketing-operations/-/blob/master/.gitlab/issue_templates/zapier_connection_request.md) on building out the automation, MktgOps will also be the ones to activate the `01 processing` campaign


### Step 4: Update the Salesforce campaign

- Now go to Salesforce.com and check the [All Campaigns by create date](https://gitlab.my.salesforce.com/701?fcf=00B4M000004oVF9) view. Sort by create date and your campaign should appear at the top. You may also search for your campaign tag in the search box. Select the campaign.
    - Change the `Campaign Owner` to your name
    - Update `Large Bucket` based on [criteria above](/handbook/marketing/marketing-operations/campaigns-and-programs/#campaign-large-buckets)
    - Update the event epic
    - Update the description
    - Update `Start Date` to the date of launch
    - Update `End Date`
    - Update `Budgeted Cost` - If cost is $0 list `1` in the `Budgeted Cost` field. - NOTE there needs to be at least a 1 value here for ROI calculations, otherwise, when you divide the pipeline by `0` you will always get `0` as the pipe2spend calculation.
    - Update `Region` and `Subregion` if you have the data available
    - Click Save
- Add the Marketo program link and SFDC campaign link to the epic.

**If utilizing Allocadia, follow these [steps](/handbook/marketing/marketing-operations/campaigns-and-programs/#step-5-update-the-salesforce-campaign---using-allocadia).**  

### Step 5: Troubleshooting:
1. Look at the `Results` tab of the smart campaign, if there are errors, you will clearly see them there.
1. If the lead is not pushing to SFDC? Make sure that the `Person Source` is not `SurveyName`
1. If existing leads are not being pulled into the program, it is likely the `SurveyName` field is capturing the wrong name.
1. If net-new leads are not being pulled into the program, it is likely the `Person Source` SurveyName was not updated correctly.

## Steps to Setup Direct Mail Campaigns

### Step 1: Create the Salesforce campaign
- Clone the [#TEMPLATE - Direct Mail](https://gitlab.my.salesforce.com/7014M000001dlh9)
- Update Campaign name to `whatever your campaign tag is`
- NOTE: You do NOT need a corresponding Marketo campaign. All information and tracking is done via this campaign.

### Step 2: Update the Salesforce campaign
- Click on `Advanced Setup` to make sure statuses correspond to those listed in the [Direct Mail progression statuses](/handbook/marketing/marketing-operations/campaigns-and-programs/#direct-mail). Do not edit these, if you need them updated, please reach out to MktgOps.
- Change the `Campaign Owner` to your name
- Confirm the `type` is `Direct Mail`
- Update `Large Bucket` based on [criteria above](/handbook/marketing/marketing-operations/campaigns-and-programs/#campaign-large-buckets)
- Update the event epic
- Update the description
- Update `Start Date` to the date of launch
- Update `End Date`
- Update `Budgeted Cost` - If cost is $0 list `1` in the `Budgeted Cost` field. - NOTE there needs to be at least a 1 value here for ROI calculations, otherwise, when you divide the pipeline by `0` you will always get `0` as the pipe2spend calculation.
- Update `Region` and `Subregion` if you have the data available
- Click Save

## Steps to Use HopIn Connector
Follow all of the set up steps to clone the template, update tokens, and update the Salesforce campaign [above](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-setup-marketo-programs-and-salesforce-campaigns). You will also need to follow the instructions below to activate the Hopin campaigns.

Important Notes:
* **YOU MUST CONNECT HOPIN TO MARKETO BEFORE YOU TURN ON REGISTRATION IN HOPIN** (STEPS 2 OR 3 BELOW)**
* To send emails using the Magic Links, you must sent the email via a smart campaign and NOT an email program. Otherwise, the join link will not properly populate. This means the confirmation email AND any reminder emails that include the join link must be sent through a smart campaign. This is built into the template.
* You must update the `{{my.hopin event name}}` and `{{my.hopin ticket code}}` tokens with information from Hopin in order for registrants to be processed correctly. Details are in the instructions below.


1. Update your Hopin-specific tokens. 
   - `{{my.hopin event name}}` - You can pull the `Event Name` from the HopIn platform - This is the name of the event exactly as it appears in Hopin.
   - `{{my.hopin ticket code}}` - Find your Ticket Integration Code in Hopin by selecting an event, and going to the Tickets page of your event dashboard. Copy the URL of the ticket name you want to use, and strip out everything but the number at the end (keep everything after the word `code=` in the URL).
     - If you are only registering for a single ticket, all you need to do is update the token, but if you have multiple ticket options, you will need to create a select dropdown in the form that holds the Integration Codes as stored values - ([ask Mops to do this for you](https://gitlab.com/gitlab-com/marketing/marketing-operations/-/issues/new#form_request)).
1. (Skip if using a marketo form) `01a Registration from Hopin` is used if you are using HopIn registration pages. This smart campaign triggers off of a custom activity `Registers for HopIn Event` and will add the registrant to the proper campaign. **THIS WILL ONLY PASS `First Name`, `Last Name`, `Email`, and the name of the event. In order to capture any of the custom fields (like company name), you'll need to set up the next step to capture registrants from Marketo. Otherwise, a dataload will be required**
   - The program token `{{my.hopin event name}}` must be populated to use this with your HopIn event name. Use `starts with` as the operator to make sure you catch all registrants. 
   - If token is updated, you can turn on. No changes are necessary for the Flow.
   - Do not turn on if you are not utilizing HopIn registration pages. You will not use this if you are using a Marketo landing page.
1. `01b. Push Registrants to Hopin from Marketo + Send Confirmation Email` is used if you are utilizing a Marketo form to capture registration for the HopIn Event. Do not turn on if you are **only** utilizing HopIn registration pages
     - Before you start with the smart campaign, you need to make sure you update the copy for the registration confirmation email named `Confirm - Hopin v2`. First, confirm all tokens on the program and then fill in the missing pieces of the email itself. Confirm that `{{member.hopin join link}}` is the CTA to the email. That will contain the link specific to each person to join the event.
        - The `{{member.hopin join link}}` token will automatically send the `Magic Link / Join Link` for the registrant to confirm their registration.
        - The magic link is automatically created by the webhook, do not update that field.
     - No changes are necessary for the campaign flow. The flow will request a Webhook, which will push the registrant into HopIn, as well as send registrant a registration confirmation email. 
    - The landing page template is already set up to have this form. You will need to change the landing page after form submit to the Thank You Page for this program. It will default to the template landing page.
     - Turn on `01b. Push Registrants to Hopin from Marketo + Send Confirmation Email`. Then test by registering on that landing page. After 3 minutes, you will recieve an email asking to confirm your registration, click the link and follow prompts on the HopIn page. Once confirmed, you will receive an email from HopIn saying it was successful. You can also look into the `attendees` section in HopIn and make sure your test is there too - once you see it, you can `remove` your test lead from the list and go live with the landing page.
1. `02 Attended Hopin` is used to track attendees of the event - it will not track individual sessions, only overall attendance.
   - To use, make sure you update the program token `{{my.hopin event name}}` with your HopIn event name. In the Smartlist, Use `starts with` as the operator to make sure you catch all registrants. 
   - When token is updated, you can turn on. No changes are necessary for the Flow.


## Steps to Setup Linkedin Lead Gen Form *Gated Content Only
We have listeners set up in Marketo listening certain parameters. Please check the `Marketo Listener` column below to see if a program is already set up in Marketo. If it is, you do not need to create a new listener, you only need to add the content to the program. Otherwise, please follow the process outlined below to ensure leads are being captured.

| Campaign                                 | Campaign Parameter for Tracking |Marketo Listener?|
|------------------------------------------|---------------------------------|-----------------|
| CI Use Case                              | singleappci                     |[Yes](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG6803A1)|
| GItOps Use Case                          | iacgitops                       |[Yes](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG6756A1)|
| Version Control & Collaboration Use Case | vccusecase                      |[Yes](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG6802A1)|
| Simplify DevOps                          | simplifydevops                  |[Yes](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG7218A1)|
| Jenkins                                  | cicdcmp2                        |[Yes](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG6976A1)|
| Increase Operational Efficiencies	       | operationalefficiences          ||
| Deliver Better Products Faster	       | betterproductsfaster            ||
| Reduce Security and Compliance Risk	   | reducesecurityrisk              ||
| CI Build & Test Auto	                   | cicdcmp3                        ||
| OctoCat	                               | octocat                         ||
| DevSecOps Use Case	                   | devsecopsusecase                | [Yes](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG9200A1)|
| AWS	                                   | awspartner                      ||
| PubSec                                   | amer-pubsec                     |[Yes](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG7588A1)|
| DevOps GTM                               | devopsgtm                       |[Yes](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG8342A1)|


If this form is in a different language, make sure that the Linkedin Form has that language in the form name (as spelled below). We currently support:
- Japanese
- Italian
- French
- Spanish
- Korean
- German
- Portuguese

When someone fills out these forms, they will be automatically added to the [Language Segmentation](/handbook/marketing/marketing-operations/marketo/#segmentations) allowing them to receive messages in their local language.


### Step 1: [Clone this Program](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG8361A1)
- Use format `YYYY_Social_[Name]_[parameter]_LinkedIn Lead Gen`
- Campaign parameter must be one of the [GTM campaign parameters](/handbook/marketing/utm-strategy/#utm-campaign) (usually used as utm_campaign - ex. `iacgitops` or `singleappci`). The Salesforce campaign name must include the campaign parameter for the responses to roll up to the correct campaign on the Sisense Demand Gen dashboard.

_e.g.: 2020_Social_GitOps_iacgitops_LinkedIn Lead Gen_

### Step 2: Sync to Salesforce

- At the program main screen in Marketo, where it says `Salesforce Sync` with "not set", click on "not set"
    - Click "Create New." The program will automatically populate the campaign tag, so you do not need to edit anything.
    - Click "Save"

### Step 3: Update the Salesforce campaign

- Now go to Salesforce.com and check the [All Campaigns by create date](https://gitlab.my.salesforce.com/701?fcf=00B4M000004oVF9) view. Sort by create date and your campaign should appear at the top. You may also search for your campaign tag in the search box. Select the campaign.
    - Change the `Campaign Owner` to your name
    - Add `Parent Campaign` of `2020_Social_LinkedIn_Lead Gen`
    - Update `Large Bucket` based on [criteria above](/handbook/marketing/marketing-operations/campaigns-and-programs/#campaign-large-buckets)
    - Update the event epic
    - Update the description
    - Update `Start Date` to the date of launch
    - Update `End Date`
    - Update `Budgeted Cost` - If cost is $0 list `1` in the `Budgeted Cost` field. - NOTE there needs to be at least a 1 value here for ROI calculations, otherwise, when you divide the pipeline by `0` you will always get `0` as the pipe2spend calculation.
    - Update `Region` and `Subregion` if you have the data available
    - Click Save
- Add the Marketo program link and SFDC campaign link to the epic.

### Step 4: Go back into Marketo Template
- Update local program tokens. Note: The template is set-up for one asset per form. If you have multiple assets, you can add additional tokens for each asset.
**Smart List**
- Update the campaign smart list filter with `contains` and the prefix
   - `Fills out Linkedin Lead Gen Form`, `Lead Gen Form Name contains [parameter]` 
   - Available parameters are [listed above](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-setup-linkedin-lead-gen-form-gated-content-only), or create new if not listed.
- `Filled out Linkedin Lead Gen Form` filter - Make sure that other programs are excluded if your new campaign will use a similar LinkedIn Lead Gen form name. Common exclusions are `amer-pubsec`, `abmkey`, and `apac-pubsec` as these flow through separate campaigns. This is not a full list of all exclusions required as this will be based on what you are setting up. You can review existing LI Lead Gen programs for examples of exclusions.
- Other programs are looking for the parameters [listed above](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-setup-linkedin-lead-gen-form-gated-content-only). If your LI Lead Gen form contains any of these, you will need to exclude your campaign from the existing program processing (for example, if your LI Lead Gen Form contains `devsecopsusecase`, you will need to exclude your LI Lead Gen form name from processing through the others that use `devsecopsusecase`). Please see the testing section below as this provides instructions to make sure you captured exclusions properly.
**Flow**
- No change to `1 - Remove from Flow` - If you remove this temporarily to test, be sure to add it back in before going live. `Remove from Flow`: Choice 1: If Email Address contains @gitlab.com. Campaign: this campaign. Default Choice: Campaign is Do nothing
- `2 - Send Email` - This step will vary. In general, you will set Choice 1: If Filled out LinkedIn Lead Gen Form contains [content name from form] then, Email [select appropriate email autoresponder]. You can have multiple choices here, one for each asset. Even if you only have one asset, best practice is to set up a choice with the default of Do Nothing. This is another backup in case the automation fails and will make sure that people don't receive an autoresponder email for another asset because the content name won't be found. You can view an example with multiple assets [here](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/SC21615C3ZN19).
- No change to `3 - Change Program Status` - This is automatically in the template. Program: [Marketo program name] - New Status Gated Content > Downloaded
- `4 - Interesting Moment` Set this up the same way as the Send Email logic, except you will change the description to match the asset. In general, you will set Choice 1: If Filled out LinkedIn Lead Gen Form contains [content name from form] then, Type Milestone, Description: Filled out LinkedIn form to view asset: [asset name]. Default choice should be generic: "Filled out LinkedIn form to view [GTM name] asset."
  - If you set up additional tokens for each asset, you can use the tokens to populate the Interesting Moments
- No changes to steps 5 and 6.
- `7 - Change Data Value` - Make sure `opt-in` language is on the Linkedin Form, if not, remove this `opt-in` step in the campaign Flow
- Turn on / Activate the triggered campaign in the `schedule` tab of the smart campaign
- All Linkedin programs with your form prefix will now flow through this campaign

### Step 5: Autoresponder email
- The autoresponder is based on tokens and will not require any changes if you only have one asset.
- If you have multiple assets, you will need to clone the autoresponder email and update all of the tokens in the email to match the additional tokens you added to the program for each asset.

### Step 6: Test your LinkedIn Lead Gen Set-up
- Have your agency (PMG or other) or Digital Marketing send a test record through the form. You can request this in the issue with the agency using the following text, updating the indicated sections:   `The Marketo program has been set-up for [name of asset] in [segment/region if applicable - you will not always need to provide this]. The automation will trigger based on [gtm code] and [content name]. Please submit a test record.`
- After the test lead is submitted, open the test record in the Marketo database. Go to the `Activity History` and confirm:
   1. The form that was submitted. You will pay attention to the gtm name and the content name. Make sure this is the form you wanted to test. If confirmed, move to step 2.
   1. Confirm the correct autoresponder for the requested asset deployed
   1. Confirm that no other autoresponders were sent
   1. Confirm that the correct Interesting Moment was triggered
   1. Confirm that the test record was added to the SFDC campaign (this may take a few minutes)
   1. Confirm that the test record was not sent any other emails or added to other programs as a result of this test

### Step 7: Update this Handbook page
- Update this [handbook page with the parameter](/handbook/marketing/marketing-operations/campaigns-and-programs/#steps-to-setup-linkedin-lead-gen-form-gated-content-only) with a `yes` and a link to the parameter and campaign you have set up.

## Raffles
Raffles can be associated with many different campaign types and have various ways to enter. You must complete the [legal requirements](https://about.gitlab.com/handbook/legal/marketing-collaboration/#engaging-legal-for-approval) before launching your raffle. 

In general, the [YYYYMMDD_SurveyName](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG6402A1) Marketo program and Survey Campaign type will be used for raffles. Due to the potential set-up complexities for raffles, Marketing Ops will need to be involved even if you use the instructions below. Use these instructions to create the program and to engage Marketing Ops for additional set-up or review.

#### For a Raffle Update Smart Lists, Flows and Tokens
- Clone the [YYYYMMDD_SurveyName](https://engage-ab.marketo.com/?munchkinId=194-VVC-221#/classic/PG6402A1)
- Name the program using the following syntax: `YYYYMMDD_NameofProgram_Raffle`. You will likely have another campaign type associated as well (for example, a Conference) and this program should be housed in the folder for that event. This is a similar process to creating a speaking session associated to a conference.
- Sync to SFDC at the program main screen in Marketo, where it says Salesforce Sync with "not set", click on "not set", Click "Create New." The program will automatically populate the campaign tag, so you do not need to edit anything except click `Save`. 
   - If you are a user of Allocadia, you will need to add the Allocadia raffle line item ID to the `Description` field. Click `Save`.
- [Update the SFDC campaign](https://about.gitlab.com/handbook/marketing/marketing-operations/campaigns-and-programs/#step-4-update-the-salesforce-campaign) and associate it to the [parent campaign](/handbook/marketing/marketing-operations/campaigns-and-programs/#parentchild-campaigns) where applicable.
   - If you are a user of Allocadia, please see instructions [here](/handbook/marketing/marketing-operations/campaigns-and-programs/#step-5-update-the-salesforce-campaign---using-allocadia).
- Go back to the Marketo program and complete the tokens. Update the {{my.Survey Name}} token with the word "Default" - do not use another entry on this token.
- If you are using a landing page: Update your [Registration page](https://about.gitlab.com/handbook/marketing/demand-generation/campaigns/landing-pages/#general-marketo-landing-page-creation-instructions), thank you page, and registration confirmation email.
- If you are using a landing page: Click into the `01a Registration Flow` and change the Smart List to "Form Name is any" and "Web page is" should already be populated with the registration page for this program. The Flow should already be populated for you, but update Step 5 - Interesting Moment to read: "Filled out form to enter raffle {{my.Survey Title}}" in the `Description` field of Step 5. Go to `Schedule` and click "Activate".
- Responders to the form will be added to the program and SFDC campaign as `Filled out Survey` and will be scored according to the `Survey - Low` entry in the [scoring model](https://about.gitlab.com/handbook/marketing/marketing-operations/marketo/#behavior-scoring).
- Due to the potential set-up complexities for raffles, Marketing Ops will need to be involved. You can add the `MktgOps::00:Triage` and `MktgOps-Support` labels to your `Marketo LP and Automation` issue for assistance with set-up.
- If you are not using a landing page, MarketingOps will help you determine the correct processing for this campaign.

## Removing Registrations from Marketo Programs

Once a landing page has been set up for a campaign, it is good practice to have multiple people test the registration to make sure everything is integrated and running properly. As a result, there are often various test registrations in the Marketo program. To remove these test registrations, follow the below instructions.

1. Log into Marketo and click into the appropriate program for your campaign
1. Click on the `Members` tab at the top of the page
1. Click on the line item for the member you wish to remove and make sure that line item is highlighted
1. Select `Change Status` at the top of the screen
1. Select `Not in Program` in the drop down 
1. Marketo will take a few moments to adjust the status and then the name will be removed from the `Members` list

### Removing SPAM from Marketo Programs and Zoom
On occassion, SPAM bots attack our webcast registration. Follow these steps to remove from Marketo and SFDC. You must open an issue with Mops to complete. Please include the marketo program link in your issue request and the dates of the event. The SPAM registrants will not be removed from zoom, and will need to be manually removed. However, it is OK to leave them in the zoom campaign, because it will not affect your campaign numbers.
1. Find the program in marketo
2. Isolate the SPAM and add them to a newly created static list.
3. Remove the SPAM from the program, by `Select All` in the static list. Then right clicking then Marketing > Change Program Status. Choose the Campaign and update the status to `Not in Program` This will also remove them from Salesforce.com campaign
4. Go to your static list. Highlight all and `Delete Person`
5. Agree to popup, and also remove from SFDC. 

After program ends, double check your Marketo program for SPAM, as people that registered (but were excluded from registration filters) would be added to program as `No Action` becuase the form is a part of that program. Re-run the steps above to fully remove them from any campaingn stats.

## Canceling an Email send
There are cases where an email is set to send, but you need to cancel it. There are a few ways to do this based on the type of program.

### Smart Campaign - Scheduled Send
1. You can cancel specific runs by going into the smart campaign > schedule and clicking the red `x` next to the date and time of send.
1. To cancel the entire run, go into the smart campaign > schedule > campaign actions > `Abort Campaign` .
   - You can still reschedule the send after you abort it

Marketo documentation:
- [Stopping campaign runs](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/cancel-a-scheduled-batch-campaign-run.html?lang=en)
- [Aborting campaign](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.html?lang=en)

### Smart Campaign - Triggered Send
1. If the campaign is running on a triggered basis, you should go into the smart campaign > schedule and click the `deactivate` button. This will stop any lead from qualifying from the campaign again.
1. If the campaign is running through multiple flow steps, in order to halt the leads from continuing in the flow, you must go into the smart campaign > schedule > campaign actions > `Abort Campaign`. This will stop leads from continuing in the flow, and stop any further emails from being sent out.

Marketo Documentation:
- [Deactivating a smart campaign](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/deactivate-a-trigger-smart-campaign-schedule-tab.html?lang=en)
- [Aborting a smart campaign](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.html?lang=en)

### Email Batch Campaign
This program type has a mailbox icon.
1. If a campaign is scheduled, but hasn't sent yet. Click into the main program (mailbox) and view the control panel. You'll see 4 boxes. In the bottom right box, click `unapprove` and the email will not go out. When you are ready to reschedule, update date and time, and click `approve` in the bottom right box. All boxes will have a green checkmark signaling it is ready for send.
1. If a campaign is actively sending and you want to stop it, click into the main program (mailbox) and in the bottom right box click `Abort Program`. This will stop the sending of emails, but will not recall any email that was already sent. You will see how many you send in the `dashboard` view. Once an email program is aborted, you cannot reschedule it again. 

You can view screenshots and further documentation from Marketo here:
- [Aborting an email program](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/abort-email-program.html?lang=en)
- [Unapproving an email program](https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/approve-unapprove-an-email-program.html?lang=en)


## Pushing DemandBase Lists to Marketo
Notes: 
- DB1 Can only pass over existing leads to Marketo, if the prospect doesn't exist in Marketo, it will be skipped.
- You still need to include email compliance filters on your email sends. This action passes a list, some people may not have consent to email.

### Checklist before initiating push to Marketo:
1. Check your list type. DB1 can only pass `person` lists, not `account` lists. 
1. Make sure your list filters contain `Compliance Segment Value` not equal to `NULL` or empty, `Default`, `Do Not Email`
1. Check your numbers on the list. The following applies:
    - **Any list over 10k** - you need ops approval to send - Add label ~"MktgOps::00: Triage" in the issue if you need to send over 10k 
    - Please try to not include over 100 people at a single account to avoid triggering SPAM filters at that account
        - Add the `Engagement Minutes` filter at the person level to get down under 100 people per account. If you send to more than 100 people per account, it will trigger spam filters.
    - For *geo wide* - i.e. all of AMER West - send should be no more than 10K
    - For *Sub-geo* - i.e all of NorCal - no more than 5k sends
    - For *territory* - i.e. Bay Area - no more than 2,500k


### Instructions:  (some lists and campaigns may already exist, we are in the process of updating templates to speed up this process) 
[Refer to this video](https://www.youtube.com/watch?v=pjL1nNheheA&list=PL05JrBw4t0KrFeuJ4JbrDZKlp6gWX0uFf&index=6) for a walkthrough of the below steps.

1. Ensure your list fits the criteria above.
1. Navigate to the Marketo Program that you would like to add your DB1 list to.
1. Under the `Lists` folder, find the list called `DB Push List - [Update event name]`. Click on this list and change `[Update event name]` to the name of your event. 
     1. If there is no list already created, create a static list by right-clicking on `Lists` and then click `New Local Asset` and select `List` from the pop up box. Name your new list`DB List Push - Name of your Event`. No `Description` is needed. Click `Create`.
1. A Smart Campaign has already been created in the `Smart Campaigns` folder to push the list from DB1. Under the `Smart Campaigns` folder, find the Smart Campaign called `DB1 List Push`. Click on this campaign, then click on `Flow`. Confirm that the name of the list you modified or created above is in the first flow step. Once you have confirmed this, skip to step 5.
     1. If there is no Smart Campaign for the list push, create a new smart campaign by right-clicking `Smart Campaigns` and selecting `New Campaign`. The campaign name should be easily identifiable to you, as you will be searching for it in DB1. Please use `DB` prefix so it's purpose is easily identifiable in Marketo. You do not need to fill in `Description` or click `Executable`. Click `Create`.
     1. Update the Smart List in the campaign by clicking `Smart List` at the top of the page
        1. On the right hand side of the screen, type in `Campaign` in the search field
        1. Drag `Campaign is Requested` from the right side of the page to the middle section of the page
        1. Update the source in the drop down to `Web Service API`
        1. You can add other filters here as necessary. Since your list will be made in DB1, you likely won't need any additional filters here.
    1. Update Flow by clicking on `Flow` at the top of the page
        1. Drag `Add to List` from the right side of the page to the middle of the page 
        1. Find the list you created in the step above in the drop down by typing in name of the list. Note that your list name will include the name of the program as well. For example - if your list name is DB1 List Push - East Event, the full name that will pull is 20210610_EastEvent.DB1 List Push - East Event
        1. If you need this group to have a specific member status, you can add that step as well by dragging over `Change Program Status` and update the new status. However, this is generally not recommended.
1. Turn on the program by clicking `Schedule` at the top of the page and clicking `Activate` and then `Activate` again in the pop up box. People should only pass through once.
1. Log into the DB1 platform and navigate to your list in the `Database` section of DB1 - *Must be a person list*
    1. You want to select all the names by clicking the checkbox at the top of the list next to `Name`. This will only select the page you are on so if you want to select all of the names on the list, click `Select All Rows` at the top of the list. Click the `Take Action` button.
    1. A sidebar on the right will pop up. Select `Add to Marketo Campaign` under `Partner Actions` section. Confirm that the number of records in the sidebar closely matches the number of records you selected. If it is off by a few records, this is fine. If it is off by hundreds or thousands, notify MOps before you complete the list push.
    1. Select the campaign in the drop down that you created a few steps ago. If you do not see your campaign, click the wheel next to the drop down to re-load the campaigns from Marketo. If it still does not show up, make sure that you activated the Marketo Smart Campaign in the previous steps above.
    1. Click `Confirm`
    1. Leads will momentarily populate your Marketo static list. In the sidebar, there will be a link to check the status of the push by clicking `See action history for status` and clicking `Job Status`. You can also view this in `Settings>History>Action History` in DB1. Loading the list may take some time but usually should take no longer than 15-20 minutes. Once your list is available, all the people in your list will show up under `Action Status` with a checkmark by `status`.
1. Go back to your Marketo program to make sure your list is available. To do this, go to the `List` folder and click on the list you created (DB1 List Push - East Event). Select `People` at the top of the page. This is where you will see all of the people in your list and can confirm the pull was successful.
    1. Once your list has successfully pulled to Marketo, deactivate the smart campaign. To do this, go to your Marketo program, click the `Smart Campaigns` folder on the left hand side of the screen under your program, click the name of your DB1 list push that you created steps above, click `Schedule` at the top of the page and click `Deactivate`.

Once your list is pushed from DB1 to Marketo, you will need to reference the static list that you created under the Marketo `List` folder (DB1 List Push - East Event) in your target lists. This reference is already built into the templates on the `Target List`, you only need to confirm the name of the DB list is correct in the filters. **If you are working with Verticurl:** You will want to reference the static list you created under the Marketo `List` folder (DB1 List Push - East Event) in your invite issues so they know which list to pull for your email sends. Verticurl will also make sure all the correct compliancy filters have been applied in Marketo before scheduling your send. **You still need to have the proper email compliance filters on any of your email programs.

### Instructions: How to update Conferences with more than 5,000 attendees
For conferences list loads with more than 5,000 attendees, consider not marking them as `success`. If the acting `Field Marketing Director` agrees to avoid marking these members as `success`, these are the steps to avoid that from happening. **This can only be done by a member of the MktgOps team!**
1. Open Marketo, Navigate to Admin>Tags>Channel>Conference
1. Uncheck `Success` box for `Attended` and save
1. Load the list in with the attended members
1. Once the list is done processing and campaign members are added, go back into Admin>Tags>Channel>Conference, and recheck the `Success` box for `Attended`
