---
title: 'Getting a “mail certificate name mismatch” / “cannot verify server identity” error?'
taxonomy:
    category:
        - docs
    tag:
        - 'email accounts'
---

This error usually occurs when a mail client is using using a secure connection to the mail server under a custom hostname.

For example, this could occur where you have imap.yourdomain.com pointing to imap.stackmail.com. This allows you to make a secure IMAP connection, but the SSL certificate installed on our mail servers uses the **\*.stackmail.com** hostname - and not **yourdomain.com**.

It's nothing to worry about, the certificate for **\*.stackmail.com** is expected so you can trust the certificate with the knowledge that the connection will remain encrypted. Once the ceritifcate is trusted you should not receive any further warnings, unless the certificate changes. 

>>> To avoid the warning altogether, you could change the mail client to use the stackmail.com hostnames. These are: **imap.stackmail.com**, **pop.stackmail.com** or **smtp.stackmail.com** for **IMAP**, **POP** or **SMTP** respectively.