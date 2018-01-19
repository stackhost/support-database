---
title: 'I can''t send emails!'
taxonomy:
    category:
        - docs
    tag:
        - 'email accounts'
---

There a few reasons why you may not be able to send emails:

### Your ISP is blocking port 25

If you can't send an email and you're using a commercial Internet Service Provider (ISP), they may be blocking SMTP port 25. This port is standard for sending an email. But it's also standard for sending spam, so ISPs often block it. Check to see if your ISP is blocking port 25:

* Open Command Prompt (in Windows) or Terminal (Mac OS).
* Enter the code: telnet exampleDomain.com 25
* If port 25 is not blocked then you will receive a successful 220 response. If port 25 is blocked then you will get a connection error or no response at all.
* If port 25 is blocked, you can alternatively use port 587. You will need to change this within your email client and is usually configured within "preferences" or "settings".

### Verify that your email account information and settings are correct

Make sure the email account username and password that you enter in your email client are correct. To check this information:

* Login to StackCockpit (StackCP)
* Select the package of the email account you want to find out
* Select 'Email Accounts'. Here you can change the password, and then check the new password

### Authentication

Your outgoing mail server should be set up to authenticate using your password, and should not be using SSL.

### Outgoing Mail Server

If you're using StackHost to send email, you'll need to make sure that you're using either mail.domain.tld, or smtp.stackmail.com as the outgoing mail server. In the case of mail.domain.tld, you'll want to change this to your actual domain, i.e. mail.yourdomain.com.

### Firewall/Antivirus

Strong firewall or antivirus software may be blocking emails from being sent. If you think your antivirus might be stopping emails from being sent out, the quickest solution is to temporarily disable the firewall or antivirus software. Whilst disabled, try sending a test email, see if it sends, and then turn your security software back on. If the test email sends, then you may need to review the documentation available for the firewall/software to see if there's a way to bypass the restriction.

### Email Limits

Our mail platform has several limits in place in order to protect the reputation of the mail platform and prevent large quantities of spam mails being sent. Currently our mail limits are as follows:

* Web servers: 500 emails a day.
* Mailboxes: 8000 emails a day.
* Message size/attachments: The webmail system accepts attachments up to 32MB in size, and the maximum message size in our network is 50MB.

If any of these limits are breached, then it won't be possible to send mail from that hosting package or mailbox. In the case of the message size/attachment limit, you'll simply need to look at reducing the size of the email or the attachment being sent.

### Blacklisted IP Address

If the machine you're sending mail from has a blacklisted IP address, you won't be able to send email if the provider you're sending to actively checks that particular blacklist. There are a number of tools available online that are able to tell you the IP address of your machine and whether or not that particular IP address has been blacklisted. In most cases, you'll need to request delisting from the blacklist in question.