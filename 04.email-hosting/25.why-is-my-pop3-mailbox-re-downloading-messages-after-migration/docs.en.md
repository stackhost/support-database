---
title: 'Why is my POP3 mailbox re-downloading messages after migration?'
taxonomy:
    category:
        - docs
    tag:
---

While we do everything we can to help prevent this behaviour, occasionally mailboxes that have been configured using POP3 and set to 'Leave a copy of mail' on the server may redownload all e-mail from the server, causing duplicates to exist in the mail client. During a migration, we'll always try to retain as many internal IDs of messages as possible. Unfortunately not all clients realise this.

!!!! We'd encourage POP3 users to switch to IMAP as soon as possible. In these cases - where the client was configured to leave a copy of mail on the server - all mail should already be stored on the IMAP server. You can confirm what messages the server has stored by using our webmail system.

!!! Connecting via IMAP provides many benefits. These include allowing message statuses and folders to automatically sync between all devices accessing the mailbox, and being able to access mail online via our webmail system.