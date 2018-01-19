---
title: 'Can I change my website’s PHP configuration?'
media_order: web-tools.JPG
taxonomy:
    category:
        - docs
    tag:
        - stackcp
        - cockpit
        - php
---

Yes, you can.

This is available via the Manage Hosting > Select Package > PHP Configuration section of our control panel. Alternatively, you can create a custom file in your webspace with your desired PHP configuration. Please note that PHP will only read a custom configuration once every 5 minutes, so it can take a short time before the configuration changes appear on your website. This is always the case for our WordPress platform, as PHP-FPM caches the configuration quite aggresively. 

### Control Panel

The **PHP Configuration icon** inside the control panel allows you to view and modify a list of the more common configuration options. You can also see our default values. To change one, simply enter your preferred value in the text input or make a radio selection and save.

[ui-callout]
[ui-callout-item title="Switch PHP versions" position="45%, 43%, se"]
Switch betwean many PHP versions. From 5.3 to the latest (at the time of writing - php 7.2.1)
[/ui-callout-item]
[ui-callout-item title="PHP Configuration" position="45%, 56%, sw"]
Configure currently running version the way you want.
[/ui-callout-item]
![](web-tools.JPG)
[/ui-callout]

### File System (Advanced)

If you wish to set an option that is not listed in the control panel, you can just modify the ~/public_html/.user.ini file directly via File Manager. This file is parsed in addition to our standard PHP configuration by our web server, allowing you to change almost all the PHP settings for your website. If you've already made changes via the control panel you will see those in a .user.ini already. For example "max_input_time=500" would set max_input_time to 500 seconds.

### Testing

The best way to confirm the settings are live is via **phpinfo()**. This allows you to see the current (local) and default (global) PHP configuration. 