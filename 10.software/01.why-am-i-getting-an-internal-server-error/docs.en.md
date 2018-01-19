---
title: 'Why am I getting an Internal Server Error?'
taxonomy:
    category:
        - docs
    tag:
        - software
        - application
---

A white screen or Internal Server Error (error 500) usually means a script used by your website is throwing an exception and/or fatal error. When this happens, it will be logged by our system and you can view recent errors inside the "Access/Error Log" section of our control panel. 

A '**500 Internal Server Error**' message on your site is frequently due to a mistake in the site file such as a .htaccess file or web.config file.

The first step in troubleshooting this is to check the Access/Error logs. To get these:

- Login to [StackCP](https://stackcp.com)
- Select the package that is showing the internal server error
- Select ‘Access/Error Logs’ under the ‘Logs and Stats’ section

You'll want to look at the ‘Error Logs’ section and see if you can see the file path where the issue is. For example, you may see:

> www.yourDomain.com [Tue Sep 05 09:49:41 2017] [alert] [client xx.xxx.xxx.xx:xxxxx] /home/sites/xx/x/xxxxxxxxx/.htaccess
    
### Windows

If you're running a Windows hosting package, don’t forget to recycle the app pool after making any changes to your site configuration. You can do this by logging into the hosting package, selecting ‘Application Pool’ and then selecting ‘Recycle Pool’.

### WordPress

A common cause of an interal server error on WordPress sites is if you are running an incompatible PHP version. Some errors are thrown if the server is running a version of PHP that is not compatible with the website code. We currently support PHP 5.3, 5.4, 5.5, 5.6, PHP 7.0 and 7.1 or our Linux platform. You can switch between all of these versions using the 'Switch PHP Version' icon inside the control panel

If you're running WordPress, you should check if your WordPress admin area is still accessible. This is usually accessible by visiting http://your-domain.com/wp-admin.

If it is, we'd recommend disabling each plugin and theme and revisiting the site in turn to try and identify the root cause.

Also, if your website is on our WordPress hosting platform, please note that this platform is PHP 7 only. While WordPress core is compatible with this PHP version, certain plugins and themes may not be. If so, we recommend hosting the website on our Linux platform. You can automatically migrate packages from WordPress to Linux via the 'Platform Transfer' area of [StackCP](https://stackcp.com).

### Increase the PHP Memory Limits

Sometimes the internal server error may occur if you are exhausting the PHP memory limit. You can increase this by:

- Logging in to [StackCP](https://stackcp.com).
- Select ‘PHP Configuration’
- Scrolling down until you see ‘memory_limit’. Change this to ‘1024M’, and select ‘Update PHP Configuration’
- Retry the page that was showing an internal server error by refreshing using CTRL + SHIFT + R. If this did not work then you should set the memory limit back to 512M