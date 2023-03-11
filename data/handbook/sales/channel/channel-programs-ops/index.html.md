---
layout: handbook-page-toc
title: "Channel Programs Operations"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}


### Overview
This page documents the operational information and processes for managing the Channel Program Operations.  This page does not include transactional processes, which are available on the [Channel Operations Handbook page](https://about.gitlab.com/handbook/sales/field-operations/channel-operations/).


# Partner Contracts

Partners register to join the GitLab Partner Program by registering at partners.gitlab.com.  You can find more details about the registration process on the [Channel Operations Handbook](https://about.gitlab.com/handbook/sales/field-operations/channel-operations/#partner-applicant-approval--denial---granting-portal-access) page.  As part of that process, partners are able to review and approve the GitLab partner program agreement.  For partners that do not agree to all the terms of the agreement, the Legal Request process is available to negotiate contact terms.

The following are the available partner agreements and addenda:



*   Master Partner Agreement (MPA) - This includes the primary terms and conditions for all reseller, services and referral partners.
*   Reseller Addendum - The Reseller addendum covers resale and renewal terms and conditions and must be signed by all partners reselling GitLab products and services.  
*   Referral / Services Addendum - This addendum to the MSA defines the terms and conditions for referral and services payment to partners.  All partners offering services around GitLab or partners referring, but not resellering GitLab must sign this agreement
*   Managed Services Provider Agreement - This is a special agreement for any partner that will be offering GitLab managed services.
*   Training Partner Addendum - All partners that will be offering GitLab training services utilizing GitLab training materials and train the training programs must sign this addendum.

Copies of the contract templates can be found [here](https://drive.google.com/drive/folders/1nwh6jt1TYJiida9CJb6YdexIxZZEI5UO?usp=sharing).

Partner agreements are limited to a single region (Americas, EMEA, APAC, Public Sector), unless otherwise approved by Channel leadership.

# Partner Portal Administration

Members of the Channel team are granted access to the Partner Portal Admin Console.  This console enables team members to track partner engagement and view partner data.  Partner data is synched between the Partner Portal and Salesforce, so GitLab team members that have access to Salesforce can find all the partner data there.

The Admin console capabilities include:



1. Engagement metrics - Partner portal engagement metrics, such as logins, asset usage, new accounts and web analytics can be found under the Channel Intel tab.
2. Salesforce sync - Data is synchronized between the Partner Portal and Salesforce in near real time.  As data is updated in one system, it is automatically syned to the other.  The Salesforce team, along with Channel Ops and Programs maintain the synchronization.  The CRM sync is set up under Admin Settings, CRM.  
3. Workflows - Workflows are set up to take an action based on a new partner being added to the system or updates to a partner account or user record.  Workflows are found under the Setting tab.  Workflows have been set up to notify team members of a new partner sign ups, automatically provide partners with Portal login credentials, assign journeys, update data fields and other activities.  The Channel Programs team maintains the workflows.
4. Training courses and exams are available for partners in the Portal.  The courses are maintained by Field Enablement and Channel Programs.  Once the GitLab LXP is rolled out to partners, partners will access the LXP through the portal via single sign-on.
5. Journeys are set up to assign a partner a set of specific tasks and activities.  For example, new partner users are assigned an onboarding Journey.  Journeys are set up and maintained by the Channel Programs team.

** **

# Partner Support Questions

Where do partners and CAMs submit questions?

## Slack Channels

*   #channel-sales for general sales engagement questions.
*   #channel-programs-ops for questions about the overall GitLab Partner Program, rules, governance, enablement and operational processes from deal registration through order.
*   #channel-services for questions about the partner services program and partner engagement in services opportunities.
*   #resellers for partners to submit questions.

## Email and Chatter Aliases

*   Chatter @Partner Help Desk in Salesforce from Accounts or Opportunities for help with specific internal partner-related requests.
*   [partnersupport@gitlab.com](mailto:partnersupport@gitlab.com) for external partner requests and general questions.
*   [partners@gitlab.com](mailto:partners@gitlab.com) for messages to the entire channel team.

The Partner Help Desk team has compiled a list of issues and solutions to the most common Partner Portal, application and data questions into an [FAQ doc](https://docs.google.com/document/d/1rygv7btm5dl-iQrVD30zOYWq98R0dsGYNjIHTBmczGY/edit?usp=sharing).  Please start here to address any issues. This document also includes some of the PHD current state internal processes.


# Partner Services Program Management 


## Help Your Partners Become a GitLab Certified Service Partner:

Step 1: Introduce your partners to the [GitLab Certified Service Partner Program](https://about.gitlab.com/handbook/resellers/services/#gitlab-certified-service-partner-program-overview) 

Step 2: Set an enablement plan with the partner representative that identifies their key employees who sign up for training and become certified to meet the competency requirements for the program.

Step 3: Build a business plan to incorporate GitLab as a strategic element in their service practice using our [Service Development Framework](https://about.gitlab.com/handbook/resellers/services/services-catalog/)

Note: If partners do not complete the CTP certification within 6 months of starting it, they will not be allowed to complete it.

Step 4: CAMs are required to use GitLab project features to manage their partners through the CTP certification process.

Step 5: CAMs and the PHD award partners their certifications using GitLab Issues. 

#### Process for Enrolling Partners into the GitLab Certified Training Partner Program
In order to collaborate with partner organizations, the Channel Solutions Architect group has created a sub-group named [Partners](https://gitlab.com/gitlab-com/channel/partners) under the [channels sub-group](https://gitlab.com/gitlab-com/channel) in GitLab.com where the Channel Account Managers share projects directly with our partner contacts. In order to work with a partner directly, the CAM is required to ensure there is an open sub-group for the specific partner under the [Partners sub-group](https://gitlab.com/gitlab-com/channel/partners). 
1. Check for the partner's sub-group:
    * Navigate to the [Partners](https://gitlab.com/gitlab-com/channel/partners) sub-group.
    * Click on the sub-group for the region where the partner is located.
    * Review the list of partners in that region.
2. If you did not see the partner in the sub-group for their region, create a sub-group named `Partner Company Name` with two sub-groups (collaboration and internal) under the company sub-group.
    * Please refer to the [Sub-groups documentation page](https://docs.gitlab.com/ee/user/group/subgroups/) to learn how to create sub-groups.
    * Please refer to an existing partner company sub-group and use it to as a model for the new one that you are creating.
3. Whether they had to create a new collaboration sub-group for the partner or there is an existing collboration sub-group for the partner, the CAM is required to add and/or verify that the partner primary contact is a member of the collaboration sub-group with `maintainer` permissions.  

<br>After a partner accepts an invitiation, the CAM:
1. Will open a project in the [Channel Partner's collaboration sub-group](https://gitlab.com/gitlab-com/channel/partners) using the `GitLab_Certified_Service_Partner_Program` project template.
2. Name the project "`Partner Company Name` CTP Requirements Project".
Note: There is a bug that may accidentally put the new project in the templates folder. CAMs are required to verify that the project was created in the correct sub-group by checking the path dropdown and make changes to the path to put the project in the correct sub-group.
3. Open an issue using the `CTP_Requirement_Tracking_Issue` template in that project. 
   1. The template automatically engages the GitLab Channel Services team and the GitLab Education Services Delivery team
   2. The CAM is required to assign themselves and the partner primary contact to the issue. 
   3. Each assigned team member is required to complete all sections assigned to the their job title within 6 mos of creating the tracking issue.    

The issue is designed to:
1. Set certification timeline goals
2. Track completion of all program requirements for becoming a CTP, including:
   1. Program Entry requirements
   2. Identify Certified Trainer Candidates
   2. Competency requirements
   3. Compliance requirements and setting MBO goals
   4. Legal and operational requirements
3. Facilitate internal and partner contributions to the process

When all sections of the issue are completed, the GitLab Education Services Delivery team member will close the issue and proceed with awarding the certification per the GitLab Service Partner Certifications Award Process.
## Enroll Certified Trainer Candidates 
1. Ask the Certified Trainer Candidates to open an issue in the `CTP_Requirements_Tracking_Project` using the `GitLab_Certified_Trainer_Candidate_Enrollment_Issue_for_Partners` Issue Template. 
2. Follow all instructions and complete all tasks in the sections assigned to the candidate in that issue. 

## GitLab Service Partner Certifications Award Process

Channel partners who are compliant with the Channel program are eligible to achieve Certified Service Partner Certifications. We have two Channel Service Partner Certifications: 



1. GitLab Certified Professional Services Partner (PSP)
2. GitLab Certified Training Partner (CTP)

The requirements for each GitLab Certified Service Partner certification can be found on the [Channel Services Handbook Page](https://about.gitlab.com/handbook/resellers/services/#becoming-a-certified-service-partner).




### GitLab Certified Professional Services Partner Award Process

GitLab Field Enablement Channel Program Management is responsible for granting the practitioner level badges per the [Practitioner Badging Process](https://about.gitlab.com/handbook/resellers/training/). Badges will be issued as each practitioner completes the required training and certification exam associated with the GitLab Certified Professional Services Engineer certifications through an automation between the GitLab Learn system and Credly that is managed by GitLab Education Services team. 

When a partner reaches the required number of GitLab Professional Services Engineers, the GitLab Channel Programs Team will open an issue in the [Channels](https://gitlab.com/groups/gitlab-com/channel/-/issues) project using the `Partner_Certification_Award` issue template and assign the CAM responsible for the account to that issue. The CAM and the Partner Help Desk each have tasks to complete in the issue. Instructions and templates are linked in the issue to make it easy for each team member to carry out the tasks.

Within 7 calendar days of assignment the CAM will:


1. Send the appropriate certification award email to the main Partner contact person. The award email contains the following elements:
    1. Congratulations
    2. Access to a Badge Graphic Download 
    3. Offers partners help to create a press release announcing their new certification
    4. Directs partners to our social media sharing kit to help them effectively announce their new certification per our social media kit.
2. The Issue will also be automatically be assigned to GitLab Partner Help Desk who will: 
    1. Update the partner portal account information with the new certification and include the badge on the partner locator for the account.
    2. If this is the first GitLab Certified Service Partner certification, grant the partner admin access to the GitLab Service Partner Community after the CAM has notified the partner about their new certification. [This video](https://www.brighttalk.com/webcast/18613/472279) demonstrates how.
                                                                                                                                                                                                                                                 
3. If the partner indicates they want to create a Press Release about their new Services Certification; the CAM can follow the instructions on the [Channel Marketing Page](https://about.gitlab.com/handbook/marketing/corporate-communications/#partner-requests-for-press-release-support)  to request a press release.

### GitLab Certified Training Partner Award Process

The Channel Sales Manager (CSM) team will open an issue in the [Channels](https://gitlab.com/groups/gitlab-com/channel/-/issues) project using the `Partner_Certification_Award` issue template and assign themeselves to that issue. The CSM and the Partner Help Desk (PHD) each have tasks to complete in the issue. Instructions and templates are linked in the issue to make it easy for each team member to carry out the tasks.

Within 7 calendar days of assignment the CAM will:


1. Send the appropriate certification award email to the main partner contact person. The award email contains the following elements:
    1. Congratulations
    2. Access to a Badge Graphic Download 
    3. Offers partners help to create a press release announcing their new certification
    4. Directs partners to our social media sharing kit to help them effectively announce their new certification.
2. The Issue will also be automatically assigned to the PHD who will: 
    1. Update the partner portal account information with the new certification and include the badge on the partner locator for the account.
    2. If this is the first GitLab Certified Service Partner certification, the PHD will grant the partner admin access to the GitLab Service Partner Community after the CAM has notified the partner about their new certification. [This video](https://www.brighttalk.com/webcast/18613/472279) demonstrates how.
                                                                                                                                                                                                                                                 
3. If the partner indicates they want to create a Press Release about their new Services Certification; the CAM can follow the instructions on the [Channel Marketing Page](https://about.gitlab.com/handbook/marketing/corporate-communications/#partner-requests-for-press-release-support)  to request a press release.



## Channel Service Partners as Subcontractors for GitLab Professional Services
### RACI-Master Services Agreement (MSA)



The table below describes how the GitLab Channel team will work with the GitLab Professional Services team when Channel Partners are used to deliver service engagements that were sold on GitLab paper. 

RACI= Accountable, Responsible, Consult, Inform
   

<table>
  <tr>
   <td>
Deliverable \ Ownership
   </td>
   <td>Channel Team
   </td>
   <td>Professional Services
   </td>
  </tr>
  <tr>
   <td>Onboarding process creation including how to engage with GL (contracts, accounting, collaboration/communication)
   </td>
   <td>A,R
   </td>
   <td>C,I
   </td>
  </tr>
  <tr>
   <td>Partner onboarding
   </td>
   <td>A, R
   </td>
   <td>C
   </td>
  </tr>
  <tr>
   <td>Rate cards
   </td>
   <td>C
   </td>
   <td>A, R
   </td>
  </tr>
  <tr>
   <td>Billing and invoice management for a specific project
   </td>
   <td>I
   </td>
   <td>A,R
   </td>
  </tr>
  <tr>
   <td>Coordinate delivery with a partner for a specific customer
   </td>
   <td>
   </td>
   <td>R,A,C,I
   </td>
  </tr>
  <tr>
   <td>MSA terms for subcontracting arrangement
   </td>
   <td>R,I
   </td>
   <td>A,C
   </td>
  </tr>
  <tr>
   <td>Partner SOW for project engagement
   </td>
   <td>
   </td>
   <td>A,R
   </td>
  </tr>
  <tr>
   <td>Subcontracting process (SOW, invoicing, etc.)
   </td>
   <td>C,I
   </td>
   <td>A,R
   </td>
  </tr>
  <tr>
   <td>“Bench” Relationship Management (FY22) 
   </td>
   <td>C,I
   </td>
   <td>A,R
   </td>
  </tr>
  <tr>
   <td>Vetting process for partners 
   </td>
   <td>R

   <br>(prelim vetting)
   </td>
   <td>A, R
   </td>
  </tr>
</table>



### RACI-CTP
The table below describes how the GitLab Channel team will work with the GitLab Education Services Delivery team when Channel Partners are used to deliver service engagements that were sold on GitLab paper.

RACI= Accountable, Responsible, Consult, Inform


<table>
  <tr>
   <td><strong>Deliverable \ Ownership</strong>
   </td>
   <td><strong>Channel Team</strong>
   </td>
   <td><strong> Education Services</strong>
   </td>
  </tr>
  <tr>
   <td>Onboarding process creation including how to engage with GL (contracts, accounting, collaboration/communication)
   </td>
   <td>R, A
   </td>
   <td>C, I
   </td>
  </tr>
  <tr>
   <td>Partner onboarding: GitLab Partner Program
   </td>
   <td>R, A
   </td>
   <td>C
   </td>
  </tr>
  <tr>
   <td>Learning partner and/or trainer onboarding:   CTP/subcontract list
   </td>
   <td>I
   </td>
   <td>R, A
   </td>
  </tr>
  <tr>
   <td>Rate cards (PS/EdS offerings)
   </td>
   <td>C
   </td>
   <td>R, A
   </td>
  </tr>
  <tr>
   <td>Course Content Price 
   </td>
   <td>C
   </td>
   <td>R, A
   </td>
  </tr>
  <tr>
   <td>Billing and invoice management for a specific project
   </td>
   <td>I
   </td>
   <td>R, A
   </td>
  </tr>
  <tr>
   <td>Coordinate delivery with a partner for a specific customer
   </td>
   <td>
   </td>
   <td>R, A, C, I
   </td>
  </tr>
  <tr>
   <td>MSA terms for subcontracting arrangement
   </td>
   <td>C, I
   </td>
   <td>R, A
   </td>
  </tr>
  <tr>
   <td>Partner SOW for project engagement
   </td>
   <td>
   </td>
   <td>A, R
   </td>
  </tr>
  <tr>
   <td>Subcontracting process definition (SOW, invoicing, etc.)
   </td>
   <td>C, I
   </td>
   <td>A, R
   </td>
  </tr>
  <tr>
   <td>“Bench” Relationship Management (FY22) 
   </td>
   <td>C, I
   </td>
   <td>R, A
   </td>
  </tr>
  <tr>
   <td>Vetting process for partners 
   </td>
   <td>R (prelim vetting)
   </td>
   <td>A, R
   </td>
  </tr>
  <tr>
   <td>Managing monthly reporting for Channel Excellence:
   <br>Certified Subcontractor Performance ratings
   </td>
   <td>A, C 
   </td>
   <td>R 
   </td>
  </tr>
  <tr>
   <td>Collecting Monthly Metrics
   </td>
   <td>
   </td>
   <td>A, R
   </td>
  </tr>
  <tr>
   <td>Managing monthly billing
   </td>
   <td>I
   </td>
   <td>A, R
   </td>
  </tr>
</table>






# Internal NFR Request Processes

**General NFR Request Process**

Partner fills out the NFR License Request form from the "Support" tab within the [partner portal](https://partners.gitlab.com).

This creates a new line in the associated spreadsheet.

Notification is sent from the spreadsheet to anyone who has notifications set up (see **<span style="text-decoration:underline;">Set Up Google Form Spreadsheet Notifications</span> [insert link to heading]**).

Partner Help Desk (PHD) reviews request to verify:



*   If the partner account is Authorized in Impartner
*   If there are any existing NFR licenses - check license.gitlab.com with the partner account name to see if the Partner already has any existing NFR licenses.
    *   Select Partners are allowed up to 25 licenses, Open Partners up to 10 licenses
    *   If existing licenses, set the expiration date to the same expiration date as existing license (unless this is a renewal of course)
*   If the partner has at least one employee who has completed the Solution Architect Certification or Professional Services Engineer Certification training, lab and exam (with a passing score).
    *   Check in Impartner for certifications by going to the Training tab
    *   Next to the Certification: _Solution Architect Core,_ click the number in the “Completed” column to display all certification completions and sort by account to see if a certification has been completed.
    *   Next to the Certification: _GitLab Trusted Professional Services Engineer (PSE) Certification,_ click the number in the Completed column and sort by account to see if a certification has been completed.
    *   If the partner has no certifications yet, but meets the other two eligibility criteria above, currently we can still send the NFR license, but we should encourage the partner to complete the Solution Architect Core. See sample email to Partner contact and CAM, once the license has been sent, below:

        _Subject Line: NFR License Request_


        _Hi [Partner License Contact],_


        _We just sent you an email with your NFR license, please let us know if you did not receive it. _


        _To ensure you receive the most value from this license, we encourage you or someone in your organization to complete the available parts of the Solution Architect Core certification in the Partner Portal. _


        _Please let us know if you need anything else._


        _Kind regards,_


PHD works with partner if additional information is needed.

If verified, PHD follows the **<span style="text-decoration:underline;">Creating and Sending NFR Licenses [insert link to heading]</span> **process (i.e. goes to license.gitlab.com and creates new license according to the request submitted in the form). 

When submitted, an email with the license is auto-generated to the Contact Email provided and is auto-logged under the Contact Name in Salesforce. 



*   To confirm the license has been sent, find the Contact Name in Salesforce and then view the Activity History on the contact record. The activity Subject will be _Email: GitLab Ultimate Trial License Key for..._ with the email address and a reference number.

PHD informs requestor license has been sent.

**Creating and Sending NFR Licenses**



1. Once you’ve confirmed the partner is eligible to receive NFR licenses, login to license.gitlab.com
2. Click the green button in the upper right corner “New license”
3. Enter this info at minimum: 
*   Name
*   Company
*   Email
*   Users count
*   GitLab Plan = Ultimate (default)
*   Check Trial checkbox
*   Starts at = Today’s date
*   Expires at = 1 year (unless the partner already has existing NFR licenses, then set to the expiration date of the existing license so that all licenses expire the same day and can be reviewed and renewed, if needed, at the same time) 
*   Notes = [User count] [GitLab Plan] NFR Licenses for Partner: [Insert Name]
4. Click _Create License_ button

**Access Request to Generate NFR Licenses**

In order to send NFR licenses to partners, you first need to have access to dev.gitlab.org. This access then allows you access to license.gitlab.com, where we issue NFR licenses from.

**<span style="text-decoration:underline;">Access Request for dev.gitlab.org</span>**

Create a [Single Access Request](https://gitlab.com/gitlab-com/team-member-epics/access-requests/-/issues/new?issuable_template=Single_Person_Access_Request) copying the text and updating with your own information using [this issue](https://gitlab.com/gitlab-com/team-member-epics/access-requests/-/issues/7019) as an example. 



1. Title: First and Last Name, need access to dev.gitlab.org
2. Type: Issue
3. Write: (Delete everything above Person Details)
    1. Fill in _Person Details _section with your information, no SSH key needed
    2. Under _Account Creation_ go down to the checkboxes for System name:
        1. _System name: _dev.gitlab.org
        2. _Justification for this access: _I need access to this system so that I can also login and gain access to license.gitlab.com. As a Partner Help Desk Specialist, I will be fulfilling and creating new NFR licenses for Channel Partners for their internal use/demo purposes.
    3. _When is access needed?_ Check the box next to “Within next 72 hours” and add the corresponding label in the _Labels_ section.
4. _Assignee: _Your Manager,_ _Yourself (so you can track)
5. _Labels:_ IT::to do, AR-Priority::3 (other labels will be auto-added)
6. Click _Submit Issue_ button
7. In the _Comments _section below the body of the issue, type: @gitlab-com/business-technology/team-member-enablement and then click _Comment_ to post.
8. You may also want to comment to @your manager to ask them to label _AR-Approval Manager Approved_ and _ReadyForProvisioning_
9. Once approved, it should be processed by IT-OPs within the timeframe needed

Once access is granted, you will get an email from dev.gitlab.org “Account was created for you”, make sure you open the email and click the link to set your password. 

**<span style="text-decoration:underline;">Logging in to license.gitlab.com</span>**

Once your password is set at dev.gitlab.org, go to license.gitlab.com. A login screen will appear, click the green button on the left, “Login with Gitlab” and use your email and the password you just created for dev.gitlab.org.

**<span style="text-decoration:underline;">Set Up Google Form Spreadsheet Notifications</span>**

Access the [NFR License Request Form Google Sheet ](https://docs.google.com/spreadsheets/d/1AXB3ERYQMQ3RmtweidgxR18rdlb8ZObqicanOPgWyVA/edit#gid=1914005562)and set notifications following the instructions below.

You can only set up notifications for yourself. You won’t get notifications when you make changes on your spreadsheet, but you’ll get notifications when others make changes.

Open the form as a spreadsheet in Google Sheets (click the Responses tab on the form and right below that in the top right corner, click the Sheets icon “View responses in Sheets”).

At the top of the spreadsheet, click _Tools_ and then _Notification rules_.

In the window that appears, select when you want to receive notifications. 

_Notify you when:_



*   _Any changes are made: Send notifications when someone makes a change to a spreadsheet._
*   _A user submits a form: Send notifications when someone fills out a form._

In the window that appears, select how often you want to receive notifications. 

_Notify you with:_



*   _Email - daily digest: Send a daily summary of all changes._
*   _Email - right away: Send an email for every change._

Click _Save_.


## **Channel Marketing Processes**

Complete process for submitting an MDF proposal request for funds and detailed instructions regarding the approval and claim process can be found in the [Channel Partner Handbook under MDF.](https://about.gitlab.com/handbook/resellers/#requesting-market-development-funds---mdf)

Select Partners are able to submit MDF requests via the Marketing Page in the Partner Portal. Partners should be reviewing plans with you prior to submitting an MDF request in the Portal to ensure you are aligned with the proposal.

Partner Logos may be accessed in GitLab Partner Portal in the Asset Library under Marketing. Logos are segmented so only authorized Select Partners have access to the Select Logo.

## **Channel Program Engagement Process**

When initiating a project the Channel Team needs to be engaged in each part of the project from ideation to approval.  The Channel Engagement process is depicted in Diagram 1 below:

![Channel Program Engagement Process](/images/channel-program-ops/project-charlies-angels.png)*Diagram 1*

<br>

Once approved we are ready to begin with engagement with Partner Marketing, Partner Enablement, and the [Partner Communication process](https://about.gitlab.com/handbook/sales/channel/channel-programs-ops/#partner-communications).

Table 1 outlines the DRIs responsible for each step in the Channel Program Engagement process. 

Table 1: 

<table>
<tr>
   <td>Team

   </td>
   <td>DRI

   </td>
  </tr>
  <tr>
   <td>Channel Programs

   </td>
   <td>Ed Cepulis

   </td>
  </tr>
  <tr>
   <td>Channel SA

   </td>
   <td>Adrian Waters

   </td>
  </tr>
  <tr>
   <td>Channel Operations

   </td>
   <td>Colleen Farris

   </td>
  </tr>
  <tr>
   <td>Channel Marketing 

   </td>
   <td>Coleen Greco

   </td>
  </tr>
  <tr>
   <td>Partner Enablement

   </td>
   <td>Blair Fraser

   </td>
  </tr>
  <tr>
   <td>Partner Communications

   </td>
   <td>Kim Jaeger

   </td>
  </tr>
  </table>





## **Partner Enablement Tools**
The Channel Programs and Enablement team is responsible for the maintence and management of enablement tools used to support the GitLab Partner ecosystem. The three main tools that we use are: Highspot, ImParnter(Partner Portal), and EdCast. Please reference the chart below to determine where an enablement asset should reside.

![Partner Enablement Tools](/images/channel-program-ops/Partner-Enablement-Tools.png)

## **Partner Communications**
 
The Channel Programs and Enablement team is responsible for “To Partner” Communications. 

Partners are a huge part of the GitLab go-to-market strategy.  Teams managing our product, pricing, or process changes should always consider our Partners as it puts them in the best position to be successful with GitLab customers.   
 
GitLab is contractually obligated to provide Partners with **30 days notification** of any pricing, product, or program changes. Product changes to tiering, terms, or EOA must accommodate the 30-day notice before announcing to GitLab customers, so Partners are prepared for changes and to help address customer questions/concerns. The 30 day notification period allows Partners to make required changes to pricelists, company websites, and collateral.   As you create GTM and communication plans, please add extra time for the request to the Channel Program team and account for the required 30-day notification.  
 
If you have something to be communicated to our Partners, kindly submit a **Channel Partner Announcement request** using [this template](https://gitlab.com/gitlab-com/channel/channels/-/blob/master/.gitlab/issue_templates/Channel%20Partner%20Communication%20Request.md). 

For all materials requiring legal review, please refer to the [Materials Legal Review Process](/handbook/legal/materials-legal-review-process)

The Channel Program team has a standard communication cadence and vehicles to deliver notifications to Partners. Please take into account the communication cadence and delivery dates below, we appreciate and encourage as much notification as possible to allow the team to prepare and schedule requests properly.   

 **News on Demand - Channel  Partner communication platform!** News on Demand is an add-on product to Impartner, which hosts the Partner Portal.   \
NOD is used to communicate to Partners via targeted emails and the Partner Flash Newsletter. With NOD, we are able to deliver news that is relevant to the individual user. Partners can access news archives and as a contributor, you can add articles at any time. You do not have to stress about deadlines!

**Partner Flash is 100% Targeted** - using groups, we can target the audience of each communication or email. \
  \
**Partner Flash is 100% Personalized**- Partners can choose topic preferences and delivery cadence. They can opt to receive the newsletter Daily, Weekly, Bi-Weekly or Monthly. Partners can also access Partner Flash via the “My News” tab in the Partner Portal. 

**Everyone can Contribute!** - Anyone at GitLab can create a story or article for the newsletter! If you would like to be a contributor,[ click here](https://partnerflash.gitlab.com/registration/admin/personal_profile) to fill out the request form.  Once approved, navigate to the NOD **Home Page** to access training and helpful tips.  

**Partner communication resources and standard delivery dates.** 

* **Partner Flash Newsletter** - delivered to Partner users on the **1st Thursday of the month** (occasional exceptions due to holidays or other considerations.) A Partner can elect to receive the newsletter daily, weekly, or bi-weekly. The majority of our Partners receive the newsletter Monthly. If you want to contribute an article, kindly submit it three days before publication.  
* **Partner Webcast series** - At times, Channel Programs or Channel Leadership might host a Partner webcast to announce a program change or essential updates.  Channel Marketing hosts a monthly Marketing Webcast; other Channel facing teams might elect to host a Webcast for our Partners. 
* **Partner Portal Notifications** - these alerts can go to all users or a subset; we do not find this a practical stand-alone communication vehicle. Using this notification to augment one of the above resources is more effective.
* **Special Notifications via email** - using NOD we can create a one-off notification if there is an urgent need to communicate out-of-cycle announcements or send surveys or Partner SKO/Summit notifications.  \


**How to get a hold of us:** If you have completed the [engagement process approvals](https://about.gitlab.com/handbook/sales/channel/channel-programs-ops/#channel-program-engagement-process) or have any questions regarding if/how something should be communicated, please reach out to us via the **#Channel-programs-ops** Slack channel.

**Partner Flash access** - anyone at GitLab can receive Partner Flash or contribute an article.  

* **Partners** - automatically signed up when approved and authorized via the Partner Portal.  If a Partner believes they do not have access please provide the user detail: first and last name, email address, and company name in the** #Channel-programs-ops** Slack channel, and we will investigate.  Typically we find the Partner has inadvertently opted out of communications.  \

* **Internal teams must self-register to receive Partner Flash and Partner Email communications.**
    * Use [this link](https://partnerflash.gitlab.com/login/) to register; it's pretty straightforward, but check out [these instructions](https://docs.google.com/presentation/d/1iX23o0N-G25GXfBs82JsmvLw-7Bc0_8e6Cva1o81hX0/edit#slide=id.g127a0ca15c9_0_266) if you need assistance.
    * Important:Use your GitLab email address - not a personal address.
    * Select GitLab employee in the drop-down for "Company Type".
    * Once registered, you will receive an email with instructions on how to edit your communication preferences. \

* **Become a Contributor**- If you want to be a contributor,[click here](https://partnerflash.gitlab.com/registration/admin/personal_profile) and fill out the request form.  Once approved, navigate to the NOD **Home Page**or [click here](https://docs.google.com/presentation/d/1YMMQGTk1fhEDLtFAHkrMeIsIbHIYLX3O/edit?usp=sharing&ouid=109735377270454778513&rtpof=true&sd=true) to access training and helpful tips.  


## **Partner Flash Newsletter**


### Overview

Partner Flash is a monthly newsletter that recaps important Partner-related information from the month and highlights important upcoming information. The main goal of this communication is to **help Partners ramp quickly and grow their GitLab business.**


### Target Audience

The newsletter is sent to authorized users in our Partner community, the list is gathered and updated from the Partner Portal, new users are added automaticly.


### Opportunities/Requirements

The newsletter will…

**Uphold our** [values](https://about.gitlab.com/handbook/values/)of transparency and allow anyone to contribute**



*   The newsletter is for communication, the Handbook is for documentation. This means that the newsletter will disseminate updates but lean on the Handbook (and other relevant resources) as the main source of documentation, linking back to it wherever possible. Items will also be referenced in the GitLab Partner Portal.

**Prioritize repetition, brevity, user-friendliness and added value**



*   The newsletter will focus on short lists and bullet points and will link out to more robust resources.
*   Repetition is key to adoption. We will encourage our Channel teams to talk about Partner Flash and will remind Partners in our upcoming Partner Webcast series and on the GitLab Partner portal.
*   We want Partners to value the newsletter. A key to adoption will be successfully positioning it as THE resource to learn what's new and recap important information. Everything will be tied back to the payoff to the Partner or seller when possible.
*   We must reconcile the fact that this newsletter is yet another increase in communication. We will leverage it to cut down on other communications when possible.

**Be fun to look at and read**



*   A focus on multimedia is important in order to help the newsletter break the monotony of text Partners sift through each day.
*   We will use images, gifs, emojis, and video where possible. For example, instead of doing a written win-wire, we will interview the individual and embed that 30-60 second video in the newsletter.

**Help the Channel operationalize key messages**



*   We will organize information around our 3 main value drivers when possible.
*   We will frequently reiterate Sales and Channel messages through video clips and use-case examples.

**Be an opportunity for the Partner Community to "learn themselves"**



*   A peripheral goal of the newsletter is to advertise helpful resources to the Partners. We will provide helpful information in hopes that it will encourage them to seek out the source of that information and look for additional information once there.

**Highlight _all_ aspects that make a big win possible**



*   There are a lot of new Partners and sales reps who are ramping up on GitLab, we want to provide easy to access to information to help them ramp quickly.
*   We will include context around partners and alliances when they play a role in a deal.

**Keep the onus on individuals to stay informed**



*   GitLab is asynchronous, this communication is in place to help provide quick access to relevant topics, the newsletter is not a substitute for the Handbook or other resources salespeople should be leveraging on the day-to-day.

**Be general enough to allow us to remain segment-agnostic**



*   The newsletter will include general updates and resources that are applicable to most, if not all, Partners. I
*   **Be built out in the open**
*   The newsletter content will be compiled using the News On Demand platform. Any team member is welcome to contribute or make requests. See more information in the Process section below.

**Uphold our value of "everyone can contribute" we will measure success and gather Partner feedback often.**



*   We will measure success using a combination of quantitative and qualitative success metrics. See Measurement section below.
*   Giving feedback or making requests will be easy, and all input will be considered and addressed.
*   The team is committed to upholding the value of the newsletter – information should be relevant, feedback should be actioned on, and leadership should help reiterate by pointing to it as a useful resource for their teams.


### Format

**Partner Flash -  Sections, descriptions, and _News Type_**

**Top News** - Important announcements (Program Changes)  or reminders (Example: Register for Partner Summit or SKO) we should have only ONE item in this category.  \_News type: Programs, Product, Marketing, Certifications _

**New and noteworthy resources** - Secondary announcements - services program, new training, significant Partner resources  \
_News Type: Programs, Product Updates_

**Did You Know?** - GitLab highlights or awards (Gartner Report) _Product _updates or use cases  \
News Type: _Corporate & Industry news_

**Tech Talk** - Technical content  \
_News Type: technical, product_

**Enablement Extras** - Provides competitive info for sales or information to assist in the sales process.  \
_News Type: Product, Sales _

**Marketing & More** - Highlights from the Channel Marketing team.  \
_News type: Marketing_

**What's new in GitLab?** - Reviews highlights of the latest GitLab release  \
_News Type: Product_

**Events & Announcements** - Highlighted events or webcasts for Partners. \
_News Type: Events_

**News from our Distributors** - any specific Disi notifications or events

**Team Member Spotlight** - Highlights a Channel Team Member 

**(NEW!) In Case You Missed It** - Highlight an important topic from the Partner Webcast or special announcement with link to any video or recording. \ 
_News Type: Product, Program, Technical, Sales_

**(NEW!) Partner Success!** - Partner Services success story to include: Customer problem, Partner solution, Outcome - also to be shared in Field Flash.   \
_News Type: Sales, technical, product_

**Links we love (as a footer)  \
[GitLab Partner Handbook](https://about.gitlab.com/handbook/resellers/#program-requirements-and-benefits)**

**[Events Calendar (from Impartner)](https://partners.gitlab.com/English/Partner/prm/events.aspx)**


### Process

The newsletter is sent out **on the first Thursday of each month.** 

We build the newsletter using the News On Demand platform, to request to be a contributor please follow the instructions in the Partner Communications. 


Quantitative Success Metrics



*   Email open rate - Average open rate of 35% in first 6 months.
*   Click rate - Average click rate of 5% in first 6 months.

Qualitative Success Metrics



*   Increased engagement from our Partner community/leaders and stakeholders in regards to the newsletter – feedback, requests, suggestions, etc.
*   Usefulness of newsletter content as shown by other stakeholders using newsletter content for their own work.
*   Improve the Partner section of the Handbook and the Partner Portal as a result of work on the newsletter.



## **Channels groups, projects, and labels**

**Groups** Use the GitLab.com group for epics that may include issues within and outside the Channels Team group.



*   https://gitlab.com/groups/gitlab-com/-/boards/1508300?label_name[]=Channel
*   Guidelines for Partner Folders:
    *   The partners Group is further divided into regional sub-groups
    *   Within each region sub-group Partners will get their own group
    *   Partner groups contain a collaboration project and internal project
    *   Partner employees should be explicitly invited to collaboration group
    *   Internal group should not be visible to non-GitLab employees and may contain licensing details or other sensitive information
    *   Additional projects may be created within the partner subgroup to contain code bases for prototypes or PoV
    *   Please avoid creating additional subgroups within partner groups

**Projects**



*   Create issues under the “Channels” project


**Labels**



*   **Team labels**
    *   Channel- issue initially created, used in templates, the starting point for any label that involves Channels
    *   Channel Ops - label for issues that directly impact the Channel Ops & team. DRI will be defined in the intro of the issue
    *   Channel Program - label for issues that directly impact the Dir of Channel Programs & team. DRI will be defined in the intro of the issue
    *   Channel Services- label for issues that directly impact the Channel Services Manager. DRI will be defined in the intro of the issue
    *   Channel Marketing- label for issues that directly impact the Channel Marketing team. DRI will be defined in the intro of the issue
    *   Channel Distribution- label for issues that directly impact the Distribution leader. DRI will be defined in the intro of the issue
    *   Channel GSI - label for issues that are owned by the Dir of GSI. DRI will be defined in the intro of the issue
    *   Internal Channel Enablement- label for issues that are focused on Internal Channel Enablement issues. DRI will be defined in the intro of the issue
    *   Channel Handbook Needs- label for issues that are about pending or planned Channel Handbook changes. DRI will be defined in the intro of the issue
    *   QBR - Requests from Sales QBRs
*   **Priority Weighting (using Eisenhower matrix and weighted tabs in Gitlab)**
    *   WEIGHT 1 ~ Channel Priority:1 - Home runs (high value to GitLab and high likelihood of success that align to Sales & Channel OKRs) and committed to completion within stated milestones. This category will be limited because not everything can be a priority. These are both URGENT & IMPORTANT
    *   WEIGHT 2 ~ Channel Priority:2 - Big Bets (high value to GitLab, lower time urgency, longer dependencies or lower likelihood of success) within stated milestones. These are not urgent but IMPORTANT to our success
    *   WEIGHT 3 - Channel Priority:3 - Small wins within stated milestones. These are URGENT but not strategically important. Delegate or push out
    *   WEIGHT 4 - Channel Priority:4 - Small wins that are important but high value. Should be slotted in where backlog allows
    *   WEIGHT 5 - Channel Priority:Backlog - Things in the queue not currently being worked LABEL

**DRI** To be stated in intro of issue and assigned to that person. There maybe 1 or more assignee but the DRI should be stated intro of issues



