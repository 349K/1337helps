# atk6-fake_advertise6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-fake_advertise6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-fake_advertise6 [-DHF] [-Ors] [-n count] [-w seconds] interface ip-address-advertised [target-address [mac-address-advertised [source-ip-address]]]

Advertise IPv6 address on the network (with own mac if not specified),
sending it to the all-nodes multicast address if no target address is set.
Source ip address is the address advertised if not set.

Sending options:
  -n count    send how many packets (default: forever)
  -w seconds  wait time between the packets sent (default: 5)
  -m srcmac   the srcmac address to send from (not what is advertised!
Flag options:
  -O  do NOT set the override flag (default: on)
  -r  DO set the router flag (default: off)
  -s  DO set the solicitate flag (default: off)
ND Security evasion options (can be combined):
  -H  add a hop-by-hop header
  -F  add a one shot fragment header (can be specified multiple times)
  -D  add a large destination header which fragments the packet.

~~~
