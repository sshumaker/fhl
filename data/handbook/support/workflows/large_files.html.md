---
layout: handbook-page-toc
title: Support Uploader - Handling large files from Customers
description: "Support team workflow for using the Support Uploader to receive large files from customers"
category: Handling tickets
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# Global Support Uploader

## Generating a FTP user for the customer

To generate the FTP credentials for a customer, navigate to the Zendesk Super
App:

1. Click the `Support Uploader` option.
1. Click on `Generate FTP user`.

This will trigger a pipeline to generate the user. Wait up
to 5 minutes for an internal comment to be posted containing the FTP
credentials.

If you do not see an update, please reach out to Support Operations via Slack
for assistance.

## Providing credentials to the customer

To provide the credentials to the customer, please use the
`General::Support Uploader` macro, as it contains both the formatting to use and
links to explain how to utilize it.

In the macro's output, ensure you replace `HOST`, `USERNAME` and `PASSWORD` with
the values from the internal comment (made via the Zendesk Super App).

## Accessing uploaded files

When the customer uploads files, an internal comment will be made on the ticket
the FTP user was generated for. To access the file, use the same credentials
generated previously.

## File deletion

When the ticket the FTP user was generated for is closed, the FTP user (and
associated files) will automatically be removed completely.

# US Federal Support Uploader

There is not currently a US Federal Support Uploader. Please check back in the
future for more information on it when it becomes available.

# Usage

For details on using FTP to upload/download files, please see
[Support Uploader usage](https://about.gitlab.com/support/providing-large-files/#support-uploader-usage).
