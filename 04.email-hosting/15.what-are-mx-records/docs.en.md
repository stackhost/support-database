---
title: 'What are MX records?'
taxonomy:
    category:
        - docs
    tag:
        - 'email accounts'
        - 'exchange hosting'
---

MX stands for 'mail exchanger'.

It tells a 'sending' mail server how to find the 'receiving' mail server, given in order of priority, where the lower numbers are given higher priority. The MX records for StackHost.com are 'mx.StackHost.com' with priority 1 and then 'mx2.StackHost.com' with priority 2. They are tried in that order by the sending mail server. Simply, 'mx.StackHost.com' and 'mx2.StackHost.com' are regular A records that point to the IP address of each mailserver that can handle mail for StackHost.com.