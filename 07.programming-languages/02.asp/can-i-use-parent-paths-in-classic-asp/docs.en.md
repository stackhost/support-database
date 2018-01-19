---
title: 'Can I use parent paths in Classic ASP?'
taxonomy:
    category:
        - docs
    tag:
        - asp
visible: true
---

ASP Parent Paths are disabled on the platform.

As a result Classic ASP scripts using "../" notation for includes will not work correctly. As an alternative to using parent paths in your ASP code, you can use virtual paths. Virtual paths need you to enter the full folder path from the URL root of your website. For example:

#### Mapping paths:

	<% Response.Write Server.MapPath("/test/example.asp") %>

#### Including paths:

	<!--#include virtual="/_fpclass/fpdblib.inc"-->