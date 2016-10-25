# Parked Domain

This repository provides an example site which works with the S2I builder ``getwarped/s2i-httpd-server`` and displays a teaser page for a parked domain. All requests against the domain will return the same page. Cache headers will be set to ensure that any response is never cached.

## Deploying the Site

The site can be deployed using the S2I builder by running:

```
oc new-app getwarped/s2i-httpd-server~https://github.com/getwarped/httpd-parked-domain.git --name coming-soon
```