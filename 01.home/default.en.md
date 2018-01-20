---
title: Home
media_order: stackcp-1.JPG
---

# StackHost.io Support Database

Welcome! Before we continue here are some of our (and yours) important info.

### StackHost important information and urls
|Service|Url|Description
|--|--|--|
|Stack Cockpit| [https://stackcp.com](https://stackcp.com) | access to your hosting panel |
|Stack Mail| [https://stackmail.com](https://stackmail.com) | access to webmail for any email account you create |
|Stack Status| [https://stackstatus.com](https://stackstatus.com) | Service status monitoring |

#### Stackhost.io nameservers
Set your domain name servers to:

|Stackhost.io name servers|
|-|
|`ns1.stackdns.com`|
|`ns2.stackdns.com`|
|`ns3.stackdns.com`|
|`ns4.stackdns.com`|

### Email settings
|Account settings| |
|-|-|
|Username|_email address_|
|Password|Use the email account’s password.|
|Incoming Server|imap.your-domain.tld (for POP3 use pop3.your-domain.tld)|
|IMAP Port|993 (143 for non-SSL)|
|POP3 Port|995 (110 for non-SSL)|
|Outgoing Server|smtp.your-domain.tld|
|SMTP Port|465 (25 or 587 for non-SSL)|
|Username|_email address_|
|[color=green]**Authentication is required for IMAP, POP3, and SMTP.**[/color]| |

Ok, that was it, here we go...

### No 1st level support
Wait! What? Yup, you heard it right. Here is the deal. **StackHost.io** is a "developers only" service. We do not cater to general public because our service (and servers) are customised for web developers. After much thinking on how to seperate developers from regular Joes we decided to drop 1st level support because as a developer you should be more then well versed in our everyday tasks (creating databases, connecting to them, installing apps, debugging them ...) and using tools like phpmyadmin, composer, git - if you use them. Please understand we are not primarly in hosting business. We do not have any plans on becoming the next HostGator. We are an exclusive "developers only" service for when they have that one extra project/customer that needs "SEO" boost far away from overcrowded, virus infested servers and they don't want to spend a small fortune on SEO sdvertising. 

>>>>> Ofcourse we offer `2nd level` support when you have server problems but those should be extremely rare, trust us, we use those servers for our own projects as well.
>>>>> But in any case, if you need us you will be "stalked" on every page by our `support widget` so please feel free to use it :)

### About us
**StackHost.io** was created by a group of grumpy veteran web developers (yours trully started developing in PHP in 2001) who just had enough of having to upload our projects to overcrowded servers and have zero chance of fighting for organic search positions (and than have to spend a small fortune on SEO advertising). Every time we moved hosting providers who promised "mountains" we saw it was just all the same. Virus infested servers no matter what they say. Plus we had 3 hosting providers with "real SSD" storage which turned out to be slower than a floopy disk. So we started building a small server stack (hence the name **StackHost**) to host our own projects. After few months other colleagues started asking where do we host the sites as they were fast, gooole friendly and well positioned. Turnes out majority of them had the same problem. Or in the case they did had private server it was not oprimised for "seo". So we (reluctantly at first because we didn't want to start yet another hosting service) added few more servers and told our colleagues we could host only "important" projects that need **SEO boost**, otherwise they should use "normal" hosting providers for majority of their projects. But after we filled the first few servers (50 domains per server limit) we saw that there really is a need for "developers only" service. So **StackHost.io** was born. Every aspect of our service is made for developers. We are all primarly developers during the day so please don't think of **StackHost.io** as "just another hosting provider". We are a small operation and we plan on staying that way no matter what because majority of us are "developers by heart" meaning we like programming and developing during the day rather than answering beginner questions (just like you basically). We do however have  a server limit. If we reach that number we will "close" StackHost.io for new customers rather than getting more server space.

In return for accepting our "no 1st level support" policy we offer you :
- servers build and optmised from every angle for one thing and one thing only - **organic SEO**!
- **real SSD storage**, no "BS", we were burned too many times so we made sure that you can literally **see** that we are using SSD storage.
- **public free environment** (no virus infested, pre-historic CMS-es lying around)
- clean servers (you only get one directory in your file space: public_html, that's it. no other unknown files and directories (cough. looking at you cPanel) - exception is when you start using ssh - we have to keep your key somewhere so we use classic **.ssh** directory at the same tree level as your public_html directory. Also when you change the php version we note that in .htaccess file placed outside of your root so it will not be in the way.
- **strict** installation policy (wordpress is only allowed on managed servers)
- amazing [Stack Cockpit](http://www.stackcp.com/login/demo) - control panel for the next century - we had enough of cPanel and did what we do best - coded our solution from the ground up. Again having only developers in mind. We think we did an amazing job :) we use it as well and we love it
- **Free SSL Certificate** for every hosted domain (from Let's Encrypt)
- You can switch easily betwean PHP versions (from 5.3 to the latest)
- if you use SSH (and we hope you will), once logged in you have access to all the php executables (from 5.3 to the latest), composer, git, ruby etc.

>>>> Servers are regularly scanned to impose our strict installation policy (No Wordpress outside Wordpress Managed Servers).
>>>> As we are not primarly in hosting business we really don't care. We will throw you out in a heart beat if you start doing something funny.
>>>> No **if**'s and **but**'s. We mean it.

