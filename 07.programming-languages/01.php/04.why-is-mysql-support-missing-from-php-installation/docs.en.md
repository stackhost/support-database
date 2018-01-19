---
title: 'Why is MySQL support missing from PHP installation?'
taxonomy:
    category:
        - docs
    tag:
        - php
        - mysql
---

Our web servers run PHP 7.0 as standard. In this version of PHP the MySQL module has been replaced by either the 'mysqli' or 'PDO_MySQL' extension. Read more about the MySQL extension deprecation on PHP's website. 

If you have a website using this module we recommend updating your code to use the latest modules. However, if this isn't feasible or you're utilising third party software we you can run older versions of PHP on our Linux platform. You're able to switch between PHP 5.3, 5.4, 5.5, 5.6 - all of which support the older MySQL module - by using the 'Switch PHP Version' icon inside the control panel.