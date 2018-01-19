---
title: 'What are the recommended Thunderbird Mail client settings?'
taxonomy:
    category:
        - docs
    tag:
        - 'email accounts'
---

There are various methods of connecting to mailboxes on our platform. 

>>>>>> We always recommend `IMAP` as that helps keep messages in sync between various devices and our webmail system. 

This is our recommended configuration for Thunderbird mail clients.

| Incoming Server Settings | |
|--|--|
| Server Name | imap.stackmail.com (or imap.yourdomain.tld) |
| Username | _e-mail address_ |
| Port | 993 |
| Connection security | SSL/TLS |
| Authentication method | `Normal password`|

---

| Outgoing Server Settings | |
|--|--|
| Server Name | imap.stackmail.com (or imap.yourdomain.tld) |
| Username | _e-mail address_ |
| Port | 587 |
| Connection security | STARTTLS |
| Authentication method | `Normal password`|

>>>>> If you choose to use domain-branded server names, such as mail.your-domain or imap.your-domain, the secure connection may throw a certificate warning due to a common name mismatch. This can be safely trusted and your connection will remain secure.