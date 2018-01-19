---
title: 'Can I use ‘mail.domain.tld’ in my mail client?'
taxonomy:
    category:
        - docs
    tag:
        - 'email accounts'
---

Yes, but for scale and redundancy reasons we operate each service from its own hostname. So we always recommend using the most relevent hostname for incoming and outgoing servers in mail clients. These are as follows:

!!! **IMAP:** imap.stackmail.com (or imap.domain.tld)
!!!
!!! **POP:** pop3.stackmail.com (or pop3.domain.tld)
!!!
!!! **SMTP:** smtp.stackmail.com (or smtp.domain.tld)

Any clients already using these hostnames can continue to do so when the account is moved to StackHost, and any new accounts added at StackHost will have the same functionality.

>>>>>> For compatibility reasons and to help ease migrations, we automatically setup **mail.domain.tld** for each of your packages.