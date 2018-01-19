---
title: 'Do you support WordPress Network (Multisite)?'
taxonomy:
    category:
        - docs
    tag:
        - application
        - software
        - wordpress
---

Yes! All our platforms have full support for a WordPress Network (formerly Multisite). You just need to follow the Create A Network article from the WordPress codex to get this setup.

### Additional Domains

As standard, we automatically map the 'wildcard' alias for your domains to your site. What this means is you can create subdomains such as sub.domain.com and sub2.domain.com without any additional configuration.

However, if you want to add additional domain names/subdomains to the package, you can do that inside [StackCP](https://stackcp.com) 'Manage Hosting. From there, the 'Domains' icon allows you to map additional domains to your package. For Wordpress Network to work, all domains must point to the same document_root when they are added - usually public_html.

### Activating SSL on Subdomains

We automatically map \*.domain to all your packages, so you won't need to add new subdomains to the account to get them to point to your WordPress install. However this means they aren't available for additional services like SSL Certificates and e-mail accounts.

You can take advantage of our Free SSL service for any subdomains by explicitly adding them to the package. To do this, go to 'Manage Hosting', follow the 'Subdomains' icon and add the subdomains you wish to activate SSL on. As above, for Wordpress Network to work, all domains must point to the same document_root when they are added - usually public_html. Once added, head over to the SSL/TLS icon and Activate your Free SSL.