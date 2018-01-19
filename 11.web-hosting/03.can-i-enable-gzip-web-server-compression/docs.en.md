---
title: 'Can I enable GZIP Web Server Compression?'
taxonomy:
    category:
        - docs
    tag:
        - hosting
---

Gzip is a great of compressing files for faster network transfers - helping them load faster, so improving site speed. It's also a file format. 

We encourage the use of and enable Gzip Compression by default across all of our platforms. Compression is handled automatically by our Edge Cache systems, so no configuration is needed on your part.

! **Note:** Our temporary URL system does not utilise our edge caching, so any external tests for compression against the temporary URL will show compression as disabled.
! This is expected and will not be the case when testing against your actual domain name.

### Manual Configuration

If you're experiencing problems or want to enable compression manually you can do so via a ".htaccess" file.

1. Create, or edit if one already exists a file named ".htaccess" in your public_html directory.
2. Add the following line:

		AddOutputFilterByType DEFLATE text/html text/plain text/xml text/css text/javascript application/javascript

3. Save your changes.