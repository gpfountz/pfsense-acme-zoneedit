# pfsense-acme-zoneedit
patch for adding zoneedit dns provider to acme project on pfsense

install pfSense's Patches package, then create a new custom package with settings below.  patch will modify usr/local/pkg/acme/acme.inc and create usr/local/pkg/acme/dnsapi/dns_zoneedit.sh

url: https://raw.githubusercontent.com/gpfountz/pfsense-acme-zoneedit/main/acme-zoneedit.patch

path stip count: 4

base directory: /

ignore whitespace: checked