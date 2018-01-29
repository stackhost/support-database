---
title: 'How can I modify my hosts file?'
taxonomy:
    category:
        - docs
    tag:
        - hosting
---

Your machine's local hosts file allows you to overide DNS for a particular domain or subdomain name. This is a great way to test the site ahead of changing real DNS: you're able to test the website at 20i while the rest of the internet continues to use DNS to point to the existing website.

The way to modify this file and the location of it differs by operating system. 

To modify your hosts file, you can add two entries to the file that contains the IP address that you want the site to resolve to and the IP address. Adding the following two lines, for example, would point www.domain.com and domain.com to the IP 1.2.3.4:

    1.2.3.4 domain www.domain.com

### For Windows

- Press Start and Search for 'Notepad'
- In the search results, right-click Notepad and select Run as administrator.
- Use File -> Open and navigate to the following file: c:\Windows\System32\Drivers\etc\hosts
- Make the changes (below)

### For Mac OS 10.0 to 10.6

- Open Applications > Utilities > Terminal
- Type sudo nano /etc/hosts
- Enter the administrator password
- Make the changes (below) 
- To save changes in nano, press Control+x and then y when prompted.

### For Mac OS X 10.6 through 10.11

Open Applications > Utilities > Terminal
Type sudo nano /private/etc/hosts
Enter the administrator password
Make the changes (below)
Type dscacheutil -flushcache in to Terminal and press enter.
To save changes in nano, press Control-x and then "y" when prompted.

### For Linux

- Use your favourite editor to open /etc/hosts (i.e sudo vim /etc/hosts)
- Make the changes (below)

 
### Making The Change

The hosts file takes arguments of the format:

    XX.XX.XX.XX domain.tld www.domain.tld

The IP address for the website is displayed down the right hand side of our control panel, under the 'IP Address' heading. They'll usually start with '185.151.2x.xxx':

    185.151.2x.xxx domain.tld www.domain.tld sub.domain.tld

After you add this line and save the file, your system begins resolving to the specified IP address. After testing is finished please remove these entries so you start using "real DNS" once again.

!!! It's important when making this change, to ensure you have entries for both your domain and all relevent subparts, for example if you just add an entry for "doimain.tld", then "www.domain.tld" will point the original server. 

