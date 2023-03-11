---
layout: handbook-page-toc
title: "Marketing Metrics"
description: "We use Sisense to view and analyze our marketing metrics from multiple data sources."
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Marketing Metrics

Below are the definitions of our primay Marketing Metrics.

#### Inquiry

An inquiry is a stage of the lead/contact objects in SFDC. GitLab defines inquiry as an Inbound request or response to [an outbound marketing effort](https://about.gitlab.com/handbook/marketing/marketing-operations/#lead-and-contact-statuses).

##### First Order Inquiries
Inquiries that are part of a parent account that has not made an order through GitLab are classified as first-order inquiries. To find them, we join the account table to the person table on the inquiry account ID. If the field `has_first_order_available` is true on the account object, the inquiry is first order. If the inquiry does not have an account associated with it, it is also first order.

##### Date of Inquiry
Finding when a lead became an inquiry requires accounting for leads who skipped the inquiry stage. To do this take the lesser of `inquiry_date` and `inquiry_inferred_date`.

The logic for finding when a person became an inquiry is captured in the `inquiry_reporting_date` field. It should always be used to report inquiries unless you are looking for something specific.

##### Technical Definition
Any lead or contact with `Status != to Raw` and the first date between Inquiry Date and Inquiry Inferred.
Any lead or contact from the fct_crm_person table where `Status != to Raw` and `inquiry_date` or `inquiry_inferred_date` is not null.

Example Query, this will return a list of inquiries with the date they became an inquiry:
```
  SELECT 
  dim_crm_person_id,
  sfdc_record_id,
  email_hash,
  inquiry_reporting_date
  FROM common_mart_marketing.mart_crm_person
  where 
  lower(Status) != ’raw`
  and inquiry_reporting_date is not null
```

##### Source & Metric

An Inquiry is defined by records in the [Person Mart](https://dbt.gitlabdata.com/#!/model/model.gitlab_snowflake.mart_crm_person). To find the number of inquiries, take the unique count of `email_hash`

Sisense View: [rpt_crm_person_inquiry](https://app.periscopedata.com/app/gitlab:safe-dashboard/view/rpt_crm_person_inquiry/5edb66186f094f40bc49e87694ea8e8f/edit)

#### MQL

A Marketing Qualified Lead (MQL) is a stage of the lead/contact objects in SFDC. GitLab defines an MQL as a person who is [Marketing Qualified through systematic means](https://about.gitlab.com/handbook/marketing/marketing-operations/#lead-and-contact-statuses).

##### First Order MQLs
MQLs that are part of a parent account that has not made an order through GitLab are classified as first-order MQLs. To find them, we join the account table to the person table on the MQL account ID. If the field `has_first_order_available` is true on the account, the MQL is first order. If the MQL does not have an account associated with it, it is also first order.

There is a set of fields that show information regarding the First Order (FO) status of a MQL: 
1. `Is First Order Person` - this shows whether or not the record is currently a FO record
1. `FO Intial MQL` - this shows whether or not, at the time of the `Intitial MQL DateTime` (the first time the record MQL'd), the record was a FO record
1. `FO MQL` - this shows whether or not, at the time of the `MQL DateTime` (the most recent time the record MQL'd), the record was a FO record

##### Date of MQL
Finding when a lead/contact became an MQL requires accounting for leads/contacts who skipped the MQL stage. 

To do this we take the lesser of `mql_date`(`Marketo MQL DateTime` in SFDC) and `mql_inferred_date` (`SFDC MQL DateTime` in SFDC). Note: Both of these fields are hidden from views and only the SoT fields below are visible, for simplicity and consistency. 

There are two new fields in SFDC, `MQL DateTime` that is the lesser of the above two fields and `Initial MQL DateTime` which is the SoT for the first time a record MQL'd - these are the only two fields that should be used in reporting on when a record MQLs. 

The logic for finding when a person became an MQL is captured in the `mql_reporting_date` field. The `mql_reporting_date` field should always be used to report inquiries unless you are looking for something specific.

| Field Label (SFDC)           | Field API Name           | Definition                                                                                                                            | Purpose and When to Use                                         |
|------------------------------|--------------------------|------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------|
| [Beta] MQL DateTime          | True_MQL_Date__c         | The true/reportable MQL Date for the most recent MQL of a record. Lesser of Marketo MQL DateTime and SFDC MQL DateTime                   | Current MQL Count/ When a record most recently MQL'd |
| Initial MQL DateTime         | True_Initial_MQL_Date__c | The true/reportable MQL Date for the first/initial MQL of a record. Lesser of Initial Marketo MQL DateTime and Initial SFDC MQL DateTime | When a record First MQL'd                            |
| Initial Marketo MQL DateTime | Initial_MQL_Date__c      | Set by Marketo when a record reaches the MQL Threshold. Stamped the first time this happens                                              | input metric - not needed for reporting              |
| Initial SFDC MQL DateTime    | Initial_MQL_DateTime__c  | Set by SFDC when a record skips the MQL Stage, Inquiry > Accepted for example. Stamped the first time this happens.                      | input metric - not needed for reporting              |
| Marketo MQL DateTime         | MQL_Date__c              | Set by Marketo when a record reaches the MQL Threshold.  Updates each time this happens.                                                 | input metric - not needed for reporting              |
| SFDC MQL DateTime            | MQL_DateTime_Inferred__c | Set by SFDC when a record skips the MQL Stage, Inquiry > Accepted for example. Updates each time this happens.                           | input metric - not needed for reporting              |

##### Technical Definition
Any lead or contact from the [fct_crm_person](https://dbt.gitlabdata.com/#!/model/model.gitlab_snowflake.fct_crm_person) table where the MQL first or Inferred MQL date is not null. 

This is captured in the [fct_crm_person](https://dbt.gitlabdata.com/#!/model/model.gitlab_snowflake.fct_crm_person) table by the `is_mql = TRUE`. 

Example Query, this will return a list of MQLs with the date they became an MQL:
```
  SELECT 
  dim_crm_person.dim_crm_person_id,
  dim_crm_person.sfdc_record_id,
  Dim_crm_person.email_hash,
  collate(mql_date, mql_inquiry_date) as mql_date
  FROM mart_crm_person
  where 
  is_mql = TRUE
```

##### Source

An MQL is defined by records in the [Person Mart](https://dbt.gitlabdata.com/#!/model/model.gitlab_snowflake.mart_crm_person).

Sisense Snippet: [rpt_crm_person_mql](https://app.periscopedata.com/app/gitlab:safe-dashboard/view/rpt_crm_person_mql/5e19022f569a480bb73adcef3a1d2681/edit)

#### SAO

A Sales Accepted Opportunity (SAO) is an Opportunity that has reached the accepted stage, the criteria to accept or reject an opportunity is set by sales and defined in [their handbook](https://about.gitlab.com/handbook/sales/field-operations/gtm-resources/#criteria-for-sales-accepted-opportunity-sao).

##### First Order SAOs
SFDC stamps the order type on each SAO when it is created, meaning that each SAO knows its order type. The `order_type` field stores this information.
The logic for first-order SAOs is captured in the `is_new_logo_first_order` flag. It should always be used when querying for FO SAOs. 

##### Date of SAO
To find the date the opportunity became an SAO, use the `sales_accepted_date` field.

##### Technical Definition
Any opportunity from the [fct_crm_opportunity](https://dbt.gitlabdata.com/#!/model/model.gitlab_snowflake.fct_crm_opportunity#description) table where the stage_name is not `10-Duplicate` and `is_edu_oss` is 0, and the sales_accepted_date is not null.
These conditions are captured in the `is_sao` field on the fct_crm_opportunity table.

Example Query
```
SELECT
sales_accepted_date,
dim_crm_opportunity_id
FROM mart_crm_opportunity
WHERE 
is_sao = TRUE
and is_new_logo_first_order = TRUE
```

##### Source

An SAO is defined by records in the [Opportunity Mart](https://dbt.gitlabdata.com/#!/model/model.gitlab_snowflake.mart_crm_opportunity).

##### Sisense Snippet:
[​​rpt_crm_opportunity_accepted_period_sao](https://app.periscopedata.com/app/gitlab:safe-dashboard/view/rpt_crm_opportunity_accepted_period_sao/5ea9956269564639ac39d14beae7c945/edit)

#### Closed Won Opportunity

A Closed Won Opportunity (CW) is an opportunity where the sales team won the deal.

##### First Order CW Opportunities
Because a closed-won deal is an opportunity, the order_type field stores the first order information.
When querying for First Order Closed Won, it’s best to use the `is_new_logo_first_order` flag, this ensures that all our dashboards are using the same logic to find FO CW.

##### Date of Closed Deal
To find the date the opportunity closed, use the `close_date` field.

##### Finding Net ARR for an Opportunity
When reporting on the [Net ARR](https://about.gitlab.com/handbook/sales/sales-term-glossary/arr-in-practice/) of a closed deal, we need to ensure the deal will contribute to the company's Net ARR. To this, add the `is_net_arr_closed_deal` flag as true to the query. 

##### Technical Definition
Any opportunity from the [fct_crm_opportunity](https://dbt.gitlabdata.com/#!/model/model.gitlab_snowflake.fct_crm_opportunity#description) table where the stage_name is not `10-Duplicate` and `is_edu_oss` is 0, and the `is_won` is true, and `is_closed` is true.

These conditions are captured in the `is_closed_won` field on the fct_crm_opportunity table. The `is_closed_won` field should always be used when querying for closed-won deals.

Example Query
```
SELECT
sales_accepted_date,
dim_crm_opportunity_id
FROM mart_crm_opportunity
WHERE 
is_closed_won = TRUE
and is_new_logo_first_order = TRUE
and is_net_arr_closed_deal = TRUE
```

##### Source

A CW Opportunity is defined by records in the [Opportunity Mart](https://dbt.gitlabdata.com/#!/model/model.gitlab_snowflake.mart_crm_opportunity).

Sisense Snippet: [rpt_crm_opportunity_closed_period_closed_won](https://app.periscopedata.com/app/gitlab:safe-dashboard/view/rpt_crm_opportunity_closed_period_closed_won/5e22f16719214a549899c36ffd8ff02c/edit)


## Marketing Sisense Dashboards
In [Sisense](https://app.periscopedata.com/app/gitlab/403199/Welcome-Dashboard-%F0%9F%91%8B) there are mutlipe marketing metric dashboards. You can quickly find the current source of truth dashboards by referencing the `Marketing` topic within Sisense. There are 3 topics that marketing leverages:   
1. `Marketing` - These are the actively maintained dashboards.
1. `Marketing-WIP` - These are the WIP dashboards. They can be viewed but are not reliable yet.
1. `Marketing-Archive` - These are the archived/old dashboards. They are not to make decisions off of and no longer supported.

Below you can find a few of the major dashboards in use and descriptions/links of/to them. 

### Marketing sources

To help us improve our paid and organic campaigns, we split marketing activities out by source in to Inbound and Demand Generation related activity. Inbound and Demand Generation sources use the following Google Analytics mediums for our breakdown.

#### Inbound
* Organic
* Direct/none
* Non-paid social
* Referral

#### Demand Generation
* Display
* Paid Social
* Generic Paid Search
* Branded Paid Search

### Defining Conversion Rate

There are several ways we can use conversion rate optimization to improve marketing performance on GitLab web properties. To create a common, [MECEFU](/handbook/communication/#mecefu-terms) oriented definition for our teams we use the following formulas.

**Overall conversion rate**
We use the overall conversion rate to quickly measure the effectiveness of our marketing website. This measurement helps us establish a baseline for engagement and move to update CTAs and offers across our marketing website to improve our conversion motions. This is the formula we use to arrive at the overall conversion rate.

overall conversion rate = `goal conversion events on about.gitlab.com/total sessions on about.gitlab.com`

For example, in December 2020 there were 2,829,601 sessions across our Google Analytics profile, with 23,218 goal conversion events.

Our overall conversion rate in December 2020 was 0.82% (23,218/2,829,601).

**Offer specific conversion rate** (trial, demo, etc)
We use offer specific conversion rates to help us measure the effectiveness of pages with conversion events. This includes our trial page, demo, webcasts, resources, and other pages we use to convert visitors to inquiries. We use this formula to calculate the offer conversion rate.

offer conversion rate = `offer conversion/visits to offer pages`

Looking at December 2020 again, there were 7,226 `/demo/` pageviews with 600 `demo` conversion events.

Our demo conversion rate in December 2020 was 8.3% (600/7,226).

### Marketing Metrics Dashboard

The [Marketing Metrics Dashboard](https://app.periscopedata.com/app/gitlab/798262/TD---Marketing-Metrics) is the centralized hub of all major marketing metrics and [marketing KPIs](/handbook/marketing/revenue-marketing/#revenue-marketing-kpi-definitions). It is an evergreen source of information brought in from Salesforce that is comprised of numerous individual graphs/charts and allows the viewer to quickly filter results using pre-defined filters on the dashboard itself.

### Marketing Attribution

The [Marketing Linear Attribution Dashboard](https://app.periscopedata.com/app/gitlab/556414/Marketing-Linear-Attribution) provides insight into the campaigns, channels, assets, forms and landing pages that drive our goals.

### Marketing trial sign up flow

We use a variety of methods and systems to collect leads and understand how people discover GitLab. This is a basic overview of these visitors move through marketing systems. 
Note: The time delay between a record being added to SFDC and the time it takes to process in Marketo, get a score, and get pushed back to SFDC as a MQL causes a discrepancy between Inquiries and MQLs for trials on a given day or in a given month (when the trial occurs on the first/last day of the month) when viewed on the [Marketing Metrics Dashboard](https://app.periscopedata.com/app/gitlab/431555/Marketing-Metrics).

![Trial sign up flow](/images/handbook/marketing/marketing-operations/trial-sign-up-flow.png)

### Alternative Method for Account Demographics Fields on Leads

In Q3 FY23 we completed the first phase of creating an alternative method for supplementing our Account Demographics fields on SFDC leads. We started this project after noticing a large portion of our leads had `null` values in the Account Demographics fields for segment, geo, etc.

To address this, we created and validated two new alternative mappings to account demographics fields for Segment and Geo. We took a waterfall approach, by first using the Account Demographics fields if present, then falling back to data enrichment fields on the lead record. Below is the more detialed logic:

To find Segment the logic is as follows (`employee_bucket_segment_custom`):
- If Lean_Data_Matched_Account_Sales_Segment__c shows as pubsec, use it first; otherwise use Account Demographics
- If still null, use the ZoomInfo employee count
- If still null, use the manual input employee count

To find Geo the logic is as follows (`geo_custom`):
We used the [FY23 Territories Mapping File - SSoT](https://docs.google.com/spreadsheets/d/1gElhORjqraKDMQnWzApPelyP_vVa24tAOA85vb5f3Uc/edit#gid=1236326957) mapping doc to find how countries mapped to Geos across segments.  
  - If Account Demographics, use it    
  - Otherwise find the first non-null value from Zoominfo then Cognism
  - Map the found country to a GEO via a hardcoded list.
        
This logic has been [added to DBT](https://gitlab-data.gitlab.io/analytics/#!/model/model.gitlab_snowflake.map_alternative_lead_demographics), and can be used in models as needed.

We have added new charts to the [Weekly Marketing Dashboard](https://app.periscopedata.com/app/gitlab:safe-intermediate-dashboard/965065/TD:-Weekly-Marketing-Metrics) with the alternative mappings while keeping the Account Demographics (original) version. We have also added tables to the [Integrated Marketing Dashboard](https://app.periscopedata.com/app/gitlab:safe-intermediate-dashboard/1061201/Draft:-Integrated-Marketing-v1), ensuring we left the original Account Demographics versions too.


## Filters on Marketing Dashboards
Filters are a native and integral piece of any dashboard! They allow you to quickly and easily isolate and filter your data based on pre-determined values and sets. They are of *no use* to anyone if we don't all know what a specific filter represents though! Here are the most common filters used on marketing dashboards, what data they pull from, and what they mean to you as the end-user!   

### Date Filters
1. `Group_by_Time` - this groups the X-axis dates by the specified value - either Month, Quarter, or Year
1. Fiscal Year - this groups the X-axis dates (unless noted on the chart) by GitLab's [Fiscal Years](/handbook/finance/#fiscal-year)

### Salesforce Data Filters
All of these filters pull from the linked/specified field(s) from Salesforce. Notes will indicate when there are groupings used. As all of these pull directly from SFDC and are not cleaned (except for those specified as being bucketed/grouped, anomalies may occur when our data is not properly maintained in SFDC)
1. User Segment Name - this pulls from SoT for `Segment` for each object as shown below in the [Reporting Fields Source of Truth](/handbook/marketing/strategy-performance/marketing-metrics/#reporting-fields-source-of-truth) section.
1. Source Bucket - this pulls from the `Lead Source` for Leads/Contacts as shown below in the [Reporting Fields Source of Truth](/handbook/marketing/strategy-performance/marketing-metrics/#reporting-fields-source-of-truth) section. Note: these are grouped into **buckets** which, once updatd, will be displayed in a table below. This is considered the SoT for where a specific Lead/Contact came from/was sourced.
1. Sales Qualified Source - this pulls from the [Sales Qualified Source](https://gitlab.my.salesforce.com/00N6100000HZPjd?setupid=OpportunityFields) of the Opportunity. This is considered the SoT for where an Opportunity came from/was sourced.
1. Order Type - this pulls from the [Order Type](https://gitlab.my.salesforce.com/00N4M00000Ib8Ok?setupid=OpportunityFields) field on the Opportunity. It is used to define whether an Opportunity is `New First Order`, `New Connected`, etc.
1. User Region Name - Using the [Opportunity Owner's](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=Owner&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&_CONFIRMATIONTOKEN=VmpFPSxNakF5TVMwd05DMHhObFF4TnpveE56bzBPUzR5TURGYSxWQmZIWkc5eUh2TmFZdmtNbXhOeVBSLFl6UTNNekF5&setupid=OpportunityFields) `User Region`
1. User Geo Name - Using the [Opportunity Owner's](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=Owner&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&_CONFIRMATIONTOKEN=VmpFPSxNakF5TVMwd05DMHhObFF4TnpveE56bzBPUzR5TURGYSxWQmZIWkc5eUh2TmFZdmtNbXhOeVBSLFl6UTNNekF5&setupid=OpportunityFields) `User Geo`
1. User Area Name - Using the [Opportunity Owner's](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=Owner&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&_CONFIRMATIONTOKEN=VmpFPSxNakF5TVMwd05DMHhObFF4TnpveE56bzBPUzR5TURGYSxWQmZIWkc5eUh2TmFZdmtNbXhOeVBSLFl6UTNNekF5&setupid=OpportunityFields) `User Area`

### Lead Source Buckets
To give executives a better view of lead sources and showing where leads and contact are sourced from we created a bucketed feild. Its often refered to as `lead source buckets` in Sisense.

This grouping was first used in the [CMO Plan](https://app.periscopedata.com/app/gitlab:safe-dashboard/943559/WIP:-CMO-Plan)

Below is the table mapping for each lead source and its Source Bucket.   

| Initial Source                                                                                                         | Source Bucket      |
|------------------------------------------------------------------------------------------------------------------------|--------------------|
| Advertisement                                                                                                          | paid demand gen    |
| AE Generated                                                                                                           | AE Generated       |
| CE Download                                                                                                            | product            |
| CE Usage Ping                                                                                                          | product            |
| Channel Qualified Lead                                                                                                 | partner marketing  |
| Clearbit                                                                                                               | SDR prospecting    |
| Conference                                                                                                             | paid demand gen    |
| CORE Check-Up                                                                                                          | product            |
| Datanyze                                                                                                               | SDR prospecting    |
| Demo                                                                                                                   | organic inbound    |
| DiscoverOrg                                                                                                            | SDR prospecting    |
| Drift                                                                                                                  | organic inbound    |
| Education                                                                                                              | organic inbound    |
| Email Request                                                                                                          | organic inbound    |
| Email Subscription                                                                                                     | organic inbound    |
| Employee Referral                                                                                                      | other              |
| Event Partner                                                                                                          | partner marketing  |
| Executive Roundtable                                                                                                   | paid demand gen    |
| Existing Client                                                                                                        | product            |
| External Referral                                                                                                      | product            |
| Field Event                                                                                                            | paid demand gen    |
| Gainsight                                                                                                              | product            |
| Gated Content                                                                                                          | organic inbound    |
| Gated Content -                                                                                                        | organic inbound    |
| Gated Content - Demo                                                                                                   | organic inbound    |
| Gated Content - eBook                                                                                                  | organic inbound    |
| Gated Content - General                                                                                                | organic inbound    |
| Gated Content - Report                                                                                                 | organic inbound    |
| Gated Content - Reports                                                                                                | organic inbound    |
| Gated Content - select one (you may NOT choose from an option other than these): whitepaper,report,video,eBook,general | organic inbound    |
| Gated Content - study                                                                                                  | organic inbound    |
| Gated Content - Video                                                                                                  | organic inbound    |
| Gated Content - webcast                                                                                                | organic inbound    |
| Gated Content - Whitepaper                                                                                             | organic inbound    |
| GitLab DataMart                                                                                                        | product            |
| GitLab Subscription Portal                                                                                             | product            |
| GitLab.com                                                                                                             | product            |
| hopin                                                                                                                  | paid demand gen    |
| Impartner                                                                                                              | partner marketing  |
| Investor                                                                                                               | organic inbound    |
| Leadware                                                                                                               | SDR prospecting    |
| LinkedIn                                                                                                               | SDR prospecting    |
| List - DB - GACoreUpsert - 20200706                                                                                    | SDR prospecting    |
| List - Demandbase - GACoreInsert - 20200706                                                                            | SDR prospecting    |
| List-2HCentric-DB-20200914                                                                                             | SDR prospecting    |
| Newsletter                                                                                                             | product            |
| OSS                                                                                                                    | organic inbound    |
| Other                                                                                                                  | other              |
| Owned Event                                                                                                            | paid demand gen    |
| Partner                                                                                                                | partner marketing  |
| Prof Serv Request                                                                                                      | organic inbound    |
| Promotion                                                                                                              | paid demand gen    |
| Prospecting                                                                                                            | SDR prospecting    |
| Prospecting - General                                                                                                  | SDR prospecting    |
| Prospecting - LeadIQ                                                                                                   | SDR prospecting    |
| Public Relations                                                                                                       | organic inbound    |
| Purchased List                                                                                                         | SDR prospecting    |
| Registered                                                                                                             | organic inbound    |
| Request - Contact                                                                                                      | organic inbound    |
| Request - Professional Services                                                                                        | organic inbound    |
| Request - Public Sector                                                                                                | organic inbound    |
| SDR Generated                                                                                                          | SDR prospecting    |
| Security Newsletter                                                                                                    | product            |
| Startup Application                                                                                                    | product            |
| Trial - Enterprise                                                                                                     | Trial - Enterprise |
| Trial - GitLab.com                                                                                                     | Trial - GitLab.com |
| Virtual Sponsorship                                                                                                    | paid demand gen    |
| Web                                                                                                                    | organic inbound    |
| Web Chat                                                                                                               | organic inbound    |
| Web Direct                                                                                                             | Web Direct         |
| Webcast                                                                                                                | paid demand gen    |
| Word of mouth                                                                                                          | organic inbound    |
| Workshop                                                                                                               | paid demand gen    |
| ZI-EMEA-MM-OutboundQ4-2020.08.19                                                                                       | SDR prospecting    |
| Zoominfo                                                                                                               | SDR prospecting    |

## Reporting Fields Source of Truth
This section captures and links the most often used fields in reporting so that anyone pulling a Salesforce report can and is using the correct fields and the same fields that are being used in Periscope reports/dashboards.    

Note: There is a current transition to move towards the [Territory Success Planning fields](/handbook/sales/field-operations/sales-systems/gtm-technical-documentation/)

### Lead
1. [Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Lead&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DLead%26setupid%3DLeadFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DLead&setupid=LeadFields)
1. [MQL Date](https://gitlab.my.salesforce.com/00N6100000CJuLB?setupid=LeadFields) - if this is blank, the record is *not* counted as a `MQL`
1. [Sales Segment](https://gitlab.my.salesforce.com/00N6100000HHdoa?setupid=LeadFields)

### Contact
1. [Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Contact&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DContact%26setupid%3DContactFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DContact&setupid=ContactFields)
1. [MQL Date](https://gitlab.my.salesforce.com/00N4M00000IW0Jx?setupid=ContactFields) - if this is blank, the record is *not* counted as a `MQL`
1. Sales Segment - See the Account `Sales Segment` field. 

### Account
1. `Sales Segment` - Using the [Account Owner's](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=Owner&type=Account&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DAccount%26setupid%3DAccountFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DAccount&_CONFIRMATIONTOKEN=VmpFPSxNakF5TVMwd05DMHhOMVF4TlRveE5qb3dOaTQzTnpOYSxURnIyR3gyTDhNSWx5dWJmTW1ObUxGLFl6UTNNekF5&setupid=AccountFields) - `User Segment`

### Opportunity
1. [SDR/BDR](https://gitlab.my.salesforce.com/00N6100000I1Y02?setupid=OpportunityFields)
1. [Closed Date](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=CloseDate&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields&setupid=OpportunityFields)
1. [Net ARR](https://gitlab.my.salesforce.com/00N4M00000Ib5n8?setupid=OpportunityFields)
1. [Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields)
1. [Sales Accepted Date](https://gitlab.my.salesforce.com/00N6100000HmPaK?setupid=OpportunityFields)
1. [Sales Qualified Source](https://gitlab.my.salesforce.com/00N6100000HZPjd?setupid=OpportunityFields)
1. [Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields)
1. [Order Type](https://gitlab.my.salesforce.com/00N4M00000Ib8Ok?setupid=OpportunityFields)

## Dashboard Review Videos

### [Marketing Metrics](https://app.periscopedata.com/app/gitlab/798262/TD---Marketing-Metrics)

<iframe width="560" height="315" src="https://www.youtube.com/embed/7cT_IsyWrus" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### [SDR Metrics](https://app.periscopedata.com/app/gitlab/641469/SDR-Metrics)

[Video Walkthrough](https://www.youtube.com/watch?v=ygeZvKvU9uc) (Private Video)
## Useful things to know when it comes to Sisense vs. SFDC data
Given the way that our systems are connected and synched, you may see a discrepancy in the data within Sisense vs. Sales Force.com. A few things to note: 
1. Opportunity amount will be updated immediately within sales force, but will NOT show up in Sisense until the next day, as our data synchs overnight. 
1. There is about a 7 hour time difference between Sisense and SFDC, so this time lag can also create discrepancies as well. 






