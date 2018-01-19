---
title: 'How can I show detailed ASP errors?'
taxonomy:
    category:
        - docs
    tag:
        - asp
visible: true
---

By default, Windows Server hides application errors from your website. You can override this by adding the following inside a 'web.config' file that will cause IIS to output any errors to your browser:

	<configuration>
    	<system.webServer>
        	<httpErrors errorMode="Detailed" />
    	</system.webServer>
    	<system.web>
        	<customErrors mode="Off" />
        	<compilation debug="true" />
    	</system.web>
	</configuration>

This can be helpful when debugging 500 Internal Server Errors from Windows packages.