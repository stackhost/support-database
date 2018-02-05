---
title: 'What is DNS Propagation?'
taxonomy:
    category:
        - docs
    tag:
        - hosting
        - domain
        - domains
---

When you make a change to your DNS records or update your domain(s) nameservers, you need to wait a certain amount of time before these changes are fully reflected across the internet. This is because DNS records are cached by what's known as a DNS resolver. The job of a resolver is to help speed up browsing and reduce overall traffic by reducing the number of DNS lookups that are made to translate domain names to IP addresses. The time it takes for a resolvers cache to expire and a new lookup to be made is defined as DNS propagation. 

The maximum amount of time a resolver will cache a lookup for is known as the record's 'Time to Live' (TTL) value. There are two key cases to remember when it comes to propagation and TTL values:

1. Changes to DNS Records 

If you're not changing your domain(s) nameservers but just updating records on existing nameservers, the time taken for propagation should be relatively quick. This is because the TTL for the records is being controlled by the operator of the nameserver, and it's very rare you will see a provider offering TTLs of more than 4 hours. The TTL given out by our nameservers is 3600 seconds (1 hour). So if you're making a change to your records on our nameservers it won't take long to propagate.

2. Changes to your Domain(s) Nameservers

Nameserver changes are the slowest propagating, and can take up to 48 hours to propagate worldwide. This is because nameservers' records are retrieved from the root nameservers, which most commonly give out a large TTL value of 2 days (172800 seconds) - or more - causing DNS resolvers to cache these lookups for a long time.

### Can I speed this up?

Firstly, it's good to remember that it's very rare that the resolvers you're using have just cached the record you are requesting, so in very few cases will you need to wait the full time specified by the records TTL.

The DNS resolvers most likely impacting you are those operated by your Internet Service Provider (ISP). Although rare, some ISPs ignore TTL settings, and will only update their cached records every one or two days. There's a chance a simple reboot of your Internet Router will get you another set of DNS resolvers that are yet to cache your records upon reconnection. If you're regularly waiting for DNS propagation and believe your ISP is not obeying TTL values from nameservers you may wish to consider switching to Google Public DNS . This is a free, global DNS resolution service that you can use as an alternative to your current DNS provider.

### What about the WHOIS?

Checking the WHOIS record for your domain name is a good way of confirming that your nameserver change has completed successfully at the registry. However, WHOIS records are not directly related to DNS propagation. At most, a change in the WHOIS record confirms the root nameservers should now answer with your new nameservers. The TTL value is still in effect and DNS resolvers around the world may only ask the root nameservers for any updates once the original TTL has expired.