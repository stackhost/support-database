---
title: 'What is the IP Address that my site uses for external connections?'
taxonomy:
    category:
        - docs
    tag:
        - hosting
---

Due to the distributed nature of our network, the IP address your site uses to make outbound connections will differ from the IP the domain resolves-to, and hence inbound traffic routes through.

! External connections made by shared websites will appear as from either **185.151.28.62** or **185.151.28.63**

! If you have a Scheduled Tasks/Cron Job that requires external connections, these will appear from **185.151.28.61**

!! However, the above addresses are subject to change so if possible, we'd **recommend whitelisting the IP range 185.151.28.0/22**.