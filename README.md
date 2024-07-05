# pfsense-acme-zoneedit
## patch for adding zoneedit dns provider to acme project on pfsense

patch will modify usr/local/pkg/acme/acme.inc and create usr/local/pkg/acme/dnsapi/dns_zoneedit.sh

install pfSense's Patches package, then create a new custom package with settings below.  
>url: https://raw.githubusercontent.com/gpfountz/pfsense-acme-zoneedit/main/acme-zoneedit.patch
>
>path strip count: 4
>
>base directory: /
>
>ignore whitespace: checked

Fetch patch, then apply

NOTE: if you dont see the option to apply or revert this patch, try removing usr/local/pkg/acme/dnsapi/dns_zoneedit.sh

this work is built upon https://github.com/blueslow/sslcertzoneedit

---

patch created by
- cloning pfsense FreeBSD repository
- modify usr/local/pkg/acme/acme.inc
- create usr/local/pkg/acme/dnsapi/dns_zoneedit.sh
- git format-patch -1 [commit]