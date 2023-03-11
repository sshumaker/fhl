---
layout: handbook-page-toc
title: "Post-Sales"
description: "Describes the workflow governing delivery of GitLab professional service projects."
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

The purpose of this page is to describe the workflow governing delivery of professional service projects. We will start by outlining the general workflow that is common across all service delivery categories. Then we will describe the differences for engagements that do not fit the general workflow shown below.

![ps-delivery-workflow](PS-delivery-workflow.png)

[Source](https://docs.google.com/presentation/d/1TOI2aoseBoyWYQC6-xpJVMknEncCNreSFfMvOHO7EBA/edit?usp=sharing),  internal only

<!---Update this below
GitLab professional services employs three different workflows that control projects for the following categories:  standard professional services, education, and dedicated engineers.  Each of these categories have unique attributes that warrant a different approach.--->

## 1. Pre-sales
_Note: for presales scoping and SOW signature, see the [pre-sales methodology page](/handbook/customer-success/professional-services-engineering/processes/pre-sales-methodology)_

### PS/EM Assessment
**TODO: Add content about what happens in this step**

## 2. PS Project Planning

### Resource Assignment
Resource assignment happens only after the SOW is received with Customer signature. The Sr. PS Operations team identifies delivery resources based on the needs of the engagement. 

### Sales to PS Handoff
The Project Coordinator will schedule a handoff call with the account team (SAL/AE, SA, CSM), the EM who scoped the engagement, and the delivery team (PM, PSE, Trainer, Training Coordinator). The meeting will start with the EM and account team describing the customers high-level goals, current state, and desired business outcomes. The Account team should note what the growth potential is for this customer and their strategic plan to drive that growth. These topics give the context about the customer to the delivery team to understand where there might be follow on opportunities. 

The EM will discuss in more detail the details of the engagement. The Delivery team will ask clarifying questions for what is in scope and what is out of scope. The PMs will review where the project definition document is stored, which is usually in the [Active Projects](https://drive.google.com/drive/u/0/folders/1ozPKiAlUzbKwpkscaYVTp9PVoi9hWm4U) folder under the Customer project. 

**TODO: Add or link to content about what happens in this step. E.g. List link to the skills matrix,  Show example of skills requirements breakdown that come from a scoping issue, Link to the appropriate PS Operations handbook page to show the process in mavenlink**. 

### Scheduling

The Professional Services (PS) team scheduling is processed through the Sr. PS Project Coordinator (PC).  Our PSA sytem calendar is our single source of truth for scheduing our customer and internal projects.  

Follow these steps to schedule a customer engagement.

Submit a Resource Request through Mavenlink with the following details:

* Role
* Dates to be worked
* Hours requested
* Soft or Hard allocation

The PC will review the master planning for availability and procecss the resource request.  If there is a schedule conflict the PC will provide another set of project dates.

Scheduling updates and changes follow this same process with a resource request in Mavenlink.

If a customer project has not booked, but planning/scheduling discussions need to take place, reach out to the PC to review.

#### How to schedule internal time

There are 2 project that track internal time, Creditable and Non Creditable.  If hours need to be scheduled for the projects, a comment in the project activity and mention the PC:

* Requested Dates 
* Hours requested
* Task assignment
* Soft or Hard allocation

## 3. Engagement Execution

#### Kickoff

See the details in the Project workflow section of the [PS Project Management](/handbook/customer-success/professional-services-engineering/project-mgmt/) page.

### Plan
**TODO: Add content about what happens in this step**

### Discovery
During discovery or fact finding sessions with the customer, PSEs will often have a predefined list of questions that need to be answered to to ensure we're designing and building the appropriate solution given customer constraints and requirements. It is good practice to send these question to the customer prior to the discovery call so they can be prepared for the discussion.

During the call, take notes to ensure that things that have validated or invalidated your initial assumptions have been captured. At the end of the meeting, review the things you've learned to memorialize what will be designed and built. Reiterating back your understanding of the details of the agreement instills confidence in the customer representative that we understand their requirements and can deliver what was reviewed.

After the meeting, based on meeting notes, create issues in the gitlab.com customer collaboration project outlining the work. Include Consider using a simple template with `Overview`, `Open Questions`, `Tasks`, and `Acceptance Criteria`. These can be helpful in further memorializing the scope of work with the customer and getting asynchronous feedback to open questions. Make sure the `overview` is as detailed as possible, and the `tasks` section has build-to level tasks (e.g. update congregate list() function to include data from CI sources).

### Build/Validate
The build validation step is a bit vague on purpose because it depends on what was included in the scope of the engagement. The PSE can use the [delivery kits mapped to our service offerings](/handbook/customer-success/professional-services-engineering/framework/#service-offering-framework) which include templatized discovery documents, automation software to facilitate service delivery, and templatized deliverable documents. Most of the collateral will be modified and updated right from the delivery kits so this section is intentionally light on detail.


### Train

PSEs or Technical Instructors who deliver GitLab Education Services instructor-led courses can use the following workflow to ensure smooth interactions with customers. In addition, PSEs and Technical Instructors should complete these [GitLab Certified Trainer](/handbook/customer-success/professional-services-engineering/gitlab-certified-trainer-process/) steps for each course they are scheduled to deliver.

#### Preparation steps

1. The Project Coordinator will contact the customer with a "Welcome to PS Email".  The email will include proposed training dates and training session planning meeting details, which will include the trainer in the meeting. Trainer participation in this meeting is critical -- please let the Project Coordinator know if you need the meeting to be rescheduled to ensure your attendance.

1. The Project Coordinator will use these [email communication templates](https://docs.google.com/document/d/1rJ9q9gEzsumRxDhoWEe45u70efmKA0eWNg69WONuCYs/edit?usp=sharing) to ensure communication of the key details with the customer and training participants.

1. During the training planning meeting, be sure to discuss and document all of the event logistics listed in the [Training Event Plan Template](https://docs.google.com/document/d/1huNauyfhFPvLCuo-9T7Ol3FtBDYowYxiP_T5ItP2FN4/edit?usp=sharing). The Project Coordinator will create a draft of the Training Event Plan prior to the meeting and update the document during the training planning meeting.  
   * During the training planning meeting, the following course introduction are useful to use to review training topics, Zoom teleconferencing, and system requirements.  
      * [GitLab with Git Basics course introduction](https://gitlabtrainingcontent.s3-us-west-2.amazonaws.com/GitLab+Course+Introduction-GitLab+Basics+-+Storyline+output/story.html)  
      * [GitLab CI/CD course introduction](https://gitlabtrainingcontent.s3-us-west-2.amazonaws.com/GitLab+Course+Introduction-+GitLab+CICD+-+Storyline+output/story.html)  
      * [GitLab for Project Managers course introduction](https://gitlabtrainingcontent.s3-us-west-2.amazonaws.com/GitLab+Course+Introduction-+GitLab+PM+-+Storyline+output/story.html)  
      * [GitLab Security Essentials course introduction](https://gitlabtrainingcontent.s3-us-west-2.amazonaws.com/GitLab+Course+Introduction-Security+-+Storyline+output/story.html)  
      * [GitLab System Administration Basic course introduction](https://gitlabtrainingcontent.s3-us-west-2.amazonaws.com/GitLab+Course+Introduction-+GitLab+System+Admin+-+Storyline+output/story.html)  
      * [GitLab InnerSourcing course introduction](https://gitlabtrainingcontent.s3-us-west-2.amazonaws.com/GitLab+Course+Introduction-+InnerSourcing++-+Storyline+output/story.html)  

1. The Project Coordinator will add the confirmed date(s) and start/stop time(s) for each training session to the issue.

1. The Project Coordinator will set up a Zoom Meeting or Webinar session for each session using [these set up instructions](/handbook/customer-success/professional-services-engineering/remote-training-session-setup/) and add the registration link(s) to the issue. You will receive an email message with your unique link to join the Zoom Meeting or Webinar session. Make sure to locate the Zoom information within the email message and familiarize yourself with the Zoom functionality. Here is a useful Zoom article for [Managing Attendees and Panelists in a Webinar](https://support.zoom.us/hc/en-us/articles/115004834466-Managing-attendees-and-panelists-in-a-webinar). Depending on your Zoom set up, you may want to log into https://zoom.us, go to Join a Meeting, and enter the meeting ID/webinar ID to start the Zoom session.

1. At least 2 weeks prior to the training session, the Project Coordinator will email the session registration link(s) to the customer, asking them to send the link(s) to each of the employees whom they want to attend the session(s). When each person registers, they will receive an automated confirmation email with a Zoom Meeting or Webinar join link unique to each person, along with a link to add the session to their calendar.

1. Contact the PS Instructional Designer to confirm you have the latest versions of course slides and other materials.

1. Review the train-the-trainer (T3) video for the course you are delivering.

1. Review and follow the [Instructor Pre-Training Checklist](/handbook/customer-success/professional-services-engineering/processes/delivery-checklists/) to ensure that you are properly prepared for your delivery. 

1. Review, practice, and use these [PS Remote Training Tips and Tricks](/handbook/customer-success/professional-services-engineering/remote-training-tips/).

1. Complete the GitLab Training Lab set up steps below. Make sure that you review the lab exercises and ensure that the labs are working properly prior to the first day of class. 

1. When it's time to join the Zoom Meeting or Webinar session as a presenter, use the link to join the session.

##### Training lab pre-course instructor workflow

PS uses the [GitLab Demo Cloud](http://gitlabdemo.com/) as the standard environment for hands-on course lab activities and hands-on certification assessments. Follow these steps to set up your course attendees for lab access.

**1. Register your account**
1. Self-register at [gitlabdemo.com](http://gitlabdemo.com/) to create your credentials on the GitLab instance during the automated provisioning process. This will provide you with your own user account and organization group for your own projects. This step is not specific course session, but is a required step as a GitLab team member.
1. Credentials for your course attendees will be generated  when they redeem an invitation code that you’d provide to them. In essence, we create a unique invitation code for each course session that attendees redeem on [gitlabdemo.com](http://gitlabdemo.com/) on Day 1 of the course session, and their GitLab instance credentials are generated after they enter their code.

**2. Generate invitation codes**
1. The Project Coordinator will generate the invitation code for your class using the steps below and provide the invitation code information approximately a week prior to your class start date as part of the instructor friendly reminders post within your Mavenlink project.
1. Visit gitlabdemo.com
1. Sign in with Okta
1. Click `Invitation Codes` in the top navigation.
1. Click the `Create Invitation Code` button in the top right corner.
1. Fill out the form. Your invitation code is generated and GitLab group is created when you click the green button.
1. You can see a list of previously created invitation codes and links to relevant details.
1. For any edits/extensions/etc or any custom redemption rules (different durations than our standards) make a request in the #demo-systems Slack channel

**3. Share the invitation code and access instructions below with attendees**: You can do this via an email to attendees as well as including it within their course materials, letting them know the expiration date (which is 7 days from the date you generated the code).


**Demo Cloud Access Instructions:**
1. Visit gitlabdemo.com
1. Click the blue button for redeeming the code above. An anonymous user account and password will be created.
1. Click on the red button to download your credentials (very important, don’t forget to do this since you will not be able to access this page again).
1. Click the blue button to access your group and create your first project.

**4. Training Closeout**:
1. Review the [Instructor Post-Training Checklist](/handbook/customer-success/professional-services-engineering/processes/delivery-checklists/) to ensure that you have followed all of the steps to close out your training class.
1. The Project Coordinator will download the Zoom attendee report and send a Next Steps email to the customer main point of contact using an email template located in the [email communication templates](https://docs.google.com/document/d/1rJ9q9gEzsumRxDhoWEe45u70efmKA0eWNg69WONuCYs/edit?usp=sharing).
1. <strong>For courses that have certification assessments</strong>: When an attendee submits their certification assessment, review their work in the demo lab cloud within 7 days of the attendee's submission and manually release their results using the attendee's completed Google Form. [Here are the detailed instructions](https://gitlab.com/gitlab-com/customer-success/professional-services-group/education-services/-/wikis/GitLab-Certification-Instructions) for certifying customers.

### Complete 
For training engagements, check out the [close out procedures on our operations page](/handbook/customer-success/professional-services-engineering/professional-services-operations/#training-close-out). 

For blended engagements, see the `Deploy & Close` section of our [project management page])(/handbook/customer-success/professional-services-engineering/project-mgmt/#project-workflow)

### Financial Closeout 
**TODO: Add or link to content about what happens in this step**

## 4. Customer Success

### Retrospective
The project manager should schedule a retrospective at the end of the project. Invite the accout team (SAL, AE, CSM, SA), the delivery team (PSEs, trainers, Project Coordinators), Engagement Manager who scoped the engagement, and PS Leadership team. 

The [Retrospective TEMPLATE](https://docs.google.com/document/d/1CXfnCzjF_hwapy0R-89txiFUmSmvX7jvlEqWn48zN8A/edit#heading=h.yqd5ghhhm2lh) can be used to capture notes during the meeting. 

The Retrospective meeting should be run by someone that is not intimately familiar with the execution of the project (typically PS Practice Manager or Engagement Manager). During the meeting, encourage contributions into the notes doc in real time and offer for participants to verbalize their feedback.

Toward the end of the call, gather actions and assign owners to complete those actions.

### Project Go-live/Recap Document
At the end of a project the Project leader should document the customer value drives/positive business outcomes they were looking to accomplish, what PS delivered to help them accelerate their journey, and special thanks to the project team. A [template of this write up](https://docs.google.com/document/d/1U0rOXcSEsBFRITQzIKopIspkrldl804PK08cU4onoUU/edit#) be found in the PMO templates Google Drive folder. An example can be found [here](https://docs.google.com/document/d/1ltSU_2UBKovVE6y6MxG2aKImsnIwicbYjCBS385Zx0A/edit#heading=h.huf1p7y95gl9). 

### Success Plan (CSM)
**TODO: Add or link to content about what happens in this step**

### Handoff (Support)
At the end of a small/medium sized projects or after the initial implementation phase of a large engagement, open a [support ops issue](https://gitlab.com/gitlab-com/support/support-ops/support-ops-project/-/issues/new?issuable_template=Add%20Zendesk%20Organization%20Notes%20or%20Tags%20Request) and add a link to the collaboration project architecture diagram that was deployed. The Support team will load it into a field in Zendesk to help them have context for customer support requests. 







