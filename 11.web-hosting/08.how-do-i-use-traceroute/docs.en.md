---
title: 'How do I use traceroute?'
taxonomy:
    category:
        - docs
    tag:
        - hosting
---

Traceroute is a tool used for diagnosing network-related issues. It does this by displaying the route to the destination specified - a domain name or an IP address - and records how long it takes packets to reach that destination. Occasionally we may ask you to perform a traceroute. Here's how to do it on our 3 hosting platforms:

### Windows

* Click 'Start'
* Type in ​**run** and then click on the icon that appears (a box should open)
* Type **cmd** and then press OK to open command prompt
* In the window that appears, type in: 

		tracert yourdomain.com 
        
(or the IP address depending on the issue) and then press 'Enter'.

### Apple iOS

- Browse to Applications -> Utilities -> Network Utility -> Traceroute
- Enter the domain or IP address you need to diagnose, then select Trace

### Linux

- Open a Terminal window
- Type: 

		traceroute yourdomain.com
        
(or replace 'yourdomain.com' with an IP address if requested to do so)