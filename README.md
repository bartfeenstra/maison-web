# Maison - Web

[![Build Status](https://travis-ci.org/bartfeenstra/maison.svg?branch=master)](https://travis-ci.org/bartfeenstra/maison)

This is a reverse proxy, SSL terminator, and authorization barrier.

# Runtime data
Runtime data is stored in `./data` and can be backed up. `./data/conf` contains editable configuration.

## Web services
These are defined in `./data/conf/web-services`, with each line defining a service in the form `NAME ADDRESS ...TAGS`.

# HTTP Basic Auth
Web applications can be protected using a shared user list, stored at `./data/conf/htpasswd`. To administer users, you
need the `htpasswd ` utility, found in the `apache2-tools` (APT), `httpd-tools` (YUM), or `apache2-utils` (APK)
packages.
