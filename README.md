# Maison - Web

[![Build Status](https://travis-ci.org/bartfeenstra/maison-web.svg?branch=master)](https://travis-ci.org/bartfeenstra/maison-web)

This is a reverse proxy, SSL terminator, and authorization barrier.

# Runtime data
Runtime data is stored in `./data` and can be backed up.

# HTTP Basic Auth
Web applications can be protected using a shared user list, stored at `./data/services/web/htpasswd`. To administer
users, you need the `htpasswd ` utility, found in the `apache2-tools` (APT), `httpd-tools` (YUM), or `apache2-utils`
(APK) packages.
