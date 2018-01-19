---
title: 'Why do DNS changes take 24-48 hours to propagate?'
taxonomy:
    category:
        - docs
    tag:
        - dns
---

Each domain has at least two nameservers assigned to it and these nameservers hold the records for the domain.

If a server somewhere else in the world queries the nameservers for DNS records, it will most often take a local copy of the DNS record.. This means that next time it needs to know what IP a domain resolves to, it will have the answer already stored.

Once the initial changes have been made to the two original nameservers, the changes will filter out through the rest of the servers in the world until everything else is up to date. It is this that can take 24-48 hours and is known propagation.