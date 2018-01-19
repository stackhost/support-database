---
title: 'What is CGI?'
taxonomy:
    category:
        - docs
    tag:
        - software
        - cgi
---

Common Gateway Interface (CGI) is a standard way for web servers to interface with executable programs installed on a server that generate web pages dynamically.

Such programs are known as CGI scripts or simply CGIs; they're usually written in a scripting language, but can be written in any programming language. Therefore, CGI is the interface which tells the web server how to pass data to and from an application. It is therefore seen as a server-side solution. 

CGI scripts have a typical sequence of steps:

- Read the users input form.
- Do what you want with the data.
- Write the HTML responce to STDOUT.

STDOUT refers to Standard Output and is the stream where a program writes its output data.