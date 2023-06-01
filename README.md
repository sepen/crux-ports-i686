# crux-ports-i686

Unofficial i686 Ports overlay for CRUX 3.5

> IMPORTANT NOTE:
> 
> The latest release available for CRUX i686 is 3.5. As of this version there is no longer official support for i686 architectures and the official CRUX core, opt, xorg and contrib repositories no longer receive updates for 3.5. This overlay is intended to extend the life of CRUX for the i686 architecture.
> 
> The ports in this repository are not official. Use them at your own risk.

To use these ports, download the `crux-i686.httpup` file to `/etc/ports`:
```
$ sudo wget -P /etc/ports https://raw.githubusercontent.com/sepen/crux-ports-i686/3.5/crux-i686.httpup
$ sudo ports -u crux-i686
```

You may want to list it first in `/etc/prt-get.conf` to take advantage of ports overlay:
```
###
### prt-get conf
###

# note: the order matters: the package found first is used
prtdir /usr/ports/crux-i686
prtdir /usr/ports/core
prtdir /usr/ports/opt
prtdir /usr/ports/xorg
```
