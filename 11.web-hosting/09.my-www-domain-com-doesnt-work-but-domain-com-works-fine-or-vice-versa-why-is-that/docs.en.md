---
title: 'My www.domain.com doesn''t work, but domain.com works fine (or vice-versa) - why is that?'
taxonomy:
    category:
        - docs
    tag:
        - hosting
        - domains
---

If you get this behaviour after a recent update to your website or a newly created package, you're almost certainly experiencing a DNS propagation delay which will resolve itself in a matter of hours.

The assumption is that when you previously visited your website you visited using www.domain.com and not domain.com (without the www). Thus, your DNS resolvers have the lookup of www.domain.com stored in their cache. When you try to view www.domain.com again, you get your DNS resolvers cached value which is the old IP address. However, when you checked the domain with just "domain.com" (no www) your DNS resolvers did not have an answer in their cache so fetched the new (correct) IP address for the domain - hence "domain.com" works for you but "www.domain.com" does not.

The only solution here is to wait for the cache to expire on your resolver, and then when you visit the domain again a fresh lookup with be made and the new IP will be stored. If you are using the StackDNS nameservers, this should take no longer than 1 hour. If you have recently changed your nameservers, or would like to read more about DNS propagation, please check out [What is DNS Propagation?](/web-hosting/what-is-dns-propagation)