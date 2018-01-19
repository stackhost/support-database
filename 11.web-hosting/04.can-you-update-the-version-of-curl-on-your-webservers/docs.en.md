---
title: 'Can you update the version of cURL on your webservers?'
taxonomy:
    category:
        - docs
    tag:
        - hosting
---

Occasionally, applications in your webspace may run checks to help ensure your website is secure. As part of these checks, the application reads the version number of various pieces of software on our servers. Sometimes, these version numbers are old and hence raise warnings. One of the most common examples for cURL is "You currently have version 7.19.7 of cURL installed. This version is known to have security issues. Please update to the latest cURL". 

We understand how that could worry you! However, an update is not required and your site is still secure.

Our Linux/WordPress platforms run Redhat Enterprise Operating Systems, and Redhat use a process known as 'backporting' into slightly older, stable versions of software to ensure security and stability throughout the entire operating system. Put simply, while the version number may appear to be out of date, you can be assured any security fixes have been retrospectively applied to guarantee they remain secure.

!!! To find out more about backporting, please see this article on [Backporting Security Fixes](https://access.redhat.com/security/updates/backporting) on Redhat's website.