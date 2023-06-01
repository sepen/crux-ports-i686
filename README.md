# crux-ports-i686

Unofficial i686 Ports overlay for CRUX 3.5

To use these ports, download the `i686.httpup` file to `/etc/ports`:
```
$ sudo wget -P /etc/ports https://raw.githubusercontent.com/sepen/crux-port-i686/3.5/i686.httpup
$ sudo ports -u i686
```

You may want to list it first in `/etc/prt-get.conf` to take advantage of ports overlay:
```
###
### prt-get conf
###

# note: the order matters: the package found first is used
prtdir /usr/ports/i686
prtdir /usr/ports/core
prtdir /usr/ports/opt
prtdir /usr/ports/xorg
```
