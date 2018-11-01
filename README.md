# mac-vpnc-script
[Openconnect](http://www.infradead.org/openconnect/) vpnc-script with improvements for macOS.
* Added native way for adding DNS-servers with networksetup utility
* Forced refresh of DNS-cache.
* Forced use of the native way of adding routes even if iproute2 is installed.

If after connecting you experience problems such as:
```
$ ssh my_host
ssh: Could not resolve hostname my_host: nodename nor servname provided, or not known
$ ping my_host
ping: cannot resolve my_host: Unknown host
```
but
```
$ host my_host
my_host has address <ip>
```
then probably this script will help you.
