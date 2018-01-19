---
title: 'Which PHP functions are disabled on your WordPress platform?'
taxonomy:
    category:
        - docs
    tag:
        - php
        - wordpress
visible: true
---

Our WordPress platform has been specifically designed to offer the best security, performance and reliability for WordPress.

As a result, we have specifically tuned firewall rules and layers of protection to help keep WordPress sites secure. As part of this protection, a small number of PHP functions have been disabled, as we've found that they're often used for malicious purposes. 

The following functions are disabled for security reasons:

- exec
- opcache_get_configuration
- opcache_get_status
- passthru
- parse_ini_file
- popen
- proc_open
- shell_exec
- show_source
- system

!!! In our experience, it's highly unlikely any of your plugins rely on any of the functions above. However, if you have a genuine use case for any of these functions, contact us to
!!! review the case and we'll (probably) give you permission to install WordPress on our Linux platform.