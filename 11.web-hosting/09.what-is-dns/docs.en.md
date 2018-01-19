---
title: 'What is DNS?'
taxonomy:
    category:
        - docs
    tag:
        - hosting
        - dns
---

### What is DNS?

DNS means 'Domain Name System'. It sounds very technical, but it’s actually quite simple. It’s a way for your browser (eg Firefox or Chrome) or mail client (eg Outlook or Mac Mail) to find websites and services on the internet.

Computers love numbers, but humans like names. It’s far easier for you to keep someone in your iPhone’s phonebook as John Doe rather than his number 07999333456. DNS is just the Internet’s versions of this.

You’ve probably heard of IP addresses, they’re those things you occasionally see that look like 192.168.100.2 or 4.4.4.4. They're the 'phone numbers' of the internet, and you’ve definitely seen a website or an email address: www.google.com or john.doe@hotmail.com. DNS is the 'phonebook' of the internet, matching-up website and email domain names to the actual IP addresses of the servers on the Internet.

### 'A' records

A records allow a DNS name (e.g., www.stackhost.io) to be pointed to one or more IPv4 addresses (quad - AAAA - records are used for pointing a DNS name to IPv6 addresses). These are the most common kinds of records you’ll see. The DNS name “www.stackhost.io” is an A record and it points to 185.151.28.20 which is an IPv4 address. Google has “www.google.com” which is both an A and AAAA record which point to “216.58.210.36” (IPv4) and “2a00:1450:4009:800::2004” (IPv6) respectively.

### 'CNAME' records

This stands for “canonical name” and you can only have one of these per name in a DNS zone (DNS zone basically means the domain name).

A CNAME record doesn’t point to an IP address but points to another DNS name. It’s a handy way of pointing multiple names to one place, and then only managing one set of IP addresses.

One example of a CNAME is 'webbuilder.stackcp.com' pointing to 'builder.stackcp.com' which is an A record pointing to “185.151.28.40”. So this means that you can change the IPv4 address of just 'builder' and you’ve effectively changed the address for 'webbuilder' too - very handy!

### 'MX' records

MX stands for 'mail exchanger'. It tells a 'sending' mail server how to find the 'receiving' mail server, given in order of priority, with the lowest numbers given highest priority. The MX records for Stackhost.io are 'mx.stackhost.io' with priority 1 and then 'mx2.stackhost.io' with priority 2. So they're tried in that order by the sending mail server. Simply, 'mx.stackhost.io' and 'mx.stackhost.io' are regular A records (see above) that point to the IP address of each mailserver that handles mail for stackhost.io.

### 'TXT' records

TXT (or text) records are not generally used to locate servers on the internet, but to prove to external systems that the domain is yours, or, that mail from certain hosts can originate from that domain (they’re called SPF records). It’s very unlikely that you’ll need to ever manually create a TXT record, but we offer the flexibility just in case.

### 'SRV' records

SRV (or service) records are similar to A (and CNAME and MX) records in that they are used to look up the IP addresses of servers on the Internet, but also include port and protocol information. It’s very unlikely you’ll ever need to modify these for your StackHost hosting.