---
layout: handbook-page-toc
title: 'System Criticality'
category: 'General'
description: 'Definitions and categorization of Support systems criticalities'
---

<style>
  .smaller {
    font-size: 10pt;
  }
</style>

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview
{:.no_toc}

This page defines and categorizes the Support systems criticalities.

## Requirements

* Any system using a
 <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
  [data scope](#data-scope) must be maintained by the Support Operations team.
* Any system using a
  <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
  [data scope](#data-scope) must be maintained by either the Support Operations
  team or the Support team.

## Critical System Tier

We derive our Critical System Tiers (CST) from that of security and engineering,
which can be found
[here](https://about.gitlab.com/handbook/security/security-assurance/security-risk/storm-program/critical-systems.html#determining-critical-system-tiers).

## Data scope

* <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i> Contains/handles SAFE data
* <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i> Contain/handles non-public non-SAFE data
* <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i> Contains/handles public non-SAFE data

## System Criticality Table

<!-- Might be worth making a data file and using HAML for this in the future. -->
<table>
  <thead>
    <tr>
      <th>Critical System Tier</th>
      <th>Ops Maintained</th>
      <th>Support Maintained</th>
      <th>Other/No Maintainer</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Mission Critical</td>
      <td>
        <ul style='list-style: none; padding-left: 0px;'>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <a class='smaller' href='https://gitlab.zendesk.com' target='_blank'>Zendesk Global</a>
          </li>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <a class='smaller' href='https://gitlab-federal-support.zendesk.com' target='_blank'>Zendesk US Federal</a>
          </li>
        </ul>
      </td>
      <td>
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td>Business Critical</td>
      <td>
        <ul style='list-style: none; padding-left: 0px;'>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://gitlab.pagerduty.com/' target='_blank'>Pagerduty</a>
          </li>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/support-ops/zendesk-global/zd-sfdc-sync-global' target='_blank'>ZD<>SFDC sync global</a>
          </li>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/support-ops/zendesk-us-federal/zd-sfdc-sync-us-federal' target='_blank'>ZD<>SFDC sync us-federal</a>
          </li>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/support-ops/forms/account-deletion' target='_blank'>Account Deletion Form/Processor</a>
          </li>
        </ul>
      </td>
      <td>
        <ul style='list-style: none; padding-left: 0px;'>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/mechanizer' target='_blank'>Mechanizer</a>
          </li>
        </ul>
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td>Business Operational</td>
      <td>
        <ul style='list-style: none; padding-left: 0px;'>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <a class='smaller' href='https://gitlab.unbabel.com/' target='_blank'>Unbabel</a>
          </li>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://calendly.com/' target='_blank'>Calendly</a>
          </li>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/support-ops/other-software/lnr-ir-processor' target='_blank'>Global IR Form/Processor</a>
          </li>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/support-ops/other-software/lnr-ir-processor-us-federal' target='_blank'>US Federal IR Form/Processor</a>
          </li>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://gitlab.1password.com/' target='_blank'>1Password Support Vault</a>
          </li>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <a class='smaller' href='https://zapier.com/' target='_blank'>Ticket feedback Global</a>
          </li>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/support-ops/forms/us-federal-customer-feedback' target='_blank'>Ticket feedback US Federal</a>
          </li>
        </ul>
      </td>
      <td>
        <ul style='list-style: none; padding-left: 0px;'>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/support-calendar' target='_blank'>Support OOO Calendars</a>
          </li>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/zd-dl-router' target='_blank'>Zendesk Download Router</a>
          </li>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/gitlabsos' target='_blank'>GitLabSOS</a>
          </li>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/kubesos' target='_blank'>KubeSOS</a>
          </li>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/zd-dl-wiper' target='_blank'>zd-dl-wiper</a>
          </li>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/zd-user-scripts' target='_blank'>zd-user-scripts</a>
          </li>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/forms_processor/' target='_blank'>forms-processor</a>
          </li>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/readiness/support-week-in-review' target='_blank'>SWIR</a>
          </li>
        </ul>
      </td>
      <td>
        <ul style='list-style: none; padding-left: 0px;'>
          <li>
           <i class="fas fa-star fa-fw" style="color:rgb(255,0,0);"></i>
            <i class="fas fa-exclamation-circle fa-fw" style="color:rgb(128,128,128);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/support-uploader/' target='_blank'>Support Uploader</a>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>Administrative</td>
      <td>
        <ul style='list-style: none; padding-left: 0px;'>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/team' target='_blank'>Support Team Page</a>
          </li>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/support-ops/other-software/sgg-slackbot' target='_blank'>SGG Slackbot</a>
          </li>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/adwr' target='_blank'>ADWR</a>
          </li>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/dewr' target='_blank'>DEWR</a>
          </li>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/support-ops/forms/customer-ticket-generator' target='_blank'>Customer ticket generator</a>
          </li>
        </ul>
      </td>
      <td>
        <ul style='list-style: none; padding-left: 0px;'>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/support-pairing' target='_blank'>support-pairing</a>
          </li>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/upgrade-path' target='_blank'>Upgrade path</a>
          </li>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/greenhat' target='_blank'>Greenhat</a>
          </li>
          <li>
            <i class="fas fa-square fa-fw" style="color:rgb(204,204,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/1-1-issue-generator' target='_blank'>1-1 issue generator</a>
          </li>
        </ul>
      </td>
      <td>
        <ul style='list-style: none; padding-left: 0px;'>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/fast-stats' target='_blank'>fast-stats</a>
          </li>
          <li>
            <i class="fas fa-circle fa-fw" style="color:rgb(0,255,0);"></i>
            <i class="fas fa-exclamation-circle fa-fw" style="color:rgb(128,128,128);"></i>
            <a class='smaller' href='https://gitlab.com/gitlab-com/support/toolbox/gitlabrb_sanitizer' target='_blank'>gitlab.rb sanitizer</a>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Notes about the table

* All Zendesk apps are included with the Zendesk item above
* Anything with a
  <i class="fas fa-exclamation-circle fa-fw" style="color:rgb(128,128,128);"></i>
  label means it is not maintained by anyone.
