---
title: 'What are my email sending limits?'
taxonomy:
    category:
        - docs
    tag:
        - 'email accounts'
---

### Email Account Limits

The following limits apply to all messages sent via authenticated SMTP. This will primarily be used for email sent via a mail client, but can also include mail sent via your website if configured to send via SMTP.

! We impose a limit of 8,000 messages per e-mail address per 24 hours.

! No more than 10,000 recipients per day.

! No more than 2,000 unique recipients per day.

! A single email may not be sent to more than 100 individual addresses.

!!!! As an example, if you were to send 100 emails to 5 different e-mail addresses within a 24 hour period. We would count 100 messages, 500 total recipients and 5 unique recipients.

### Web Server Limits

A limit of 500 messages per day is imposed on all e-mail sent by our web servers. E-mails sent by the web servers should be no larger than 5MB in size. This applies to all messages sent via the PHP mail() function.

### Autoresponders

An autoresponder only sends once every 8 hours per sender

### Zero Tolerance Spam Policy

!! We take a **zero tolerance** stance against the sending of unsolicited email, bulk emailing and spam. Please refer to our Acceptable Use Policy for more information.

>>>>> The distributed nature of our network means email can leave through different servers at different times. As a result, you may see periods when you can send a greater number of messages than the limits mentioned above. However, this behaviour should not be relied upon and is not supported. If you do wish to send a larger number of e-mails than any of the limits mentioned above, we would recommend looking at a specialist marketing email platforms such as SendGrid, Mailgun, or Mailjet.