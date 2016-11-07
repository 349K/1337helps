# atk6-four2six command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-four2six v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-four2six [-FHD] [-m srcmac] [-s src6] [-p srcport] interface ipv6-to-ipv4-gateway ipv4-src ipv4-dst [port]

Options:
  -F         insert atomic fragment header (can be set multiple times)
  -H         insert and empty hop-by-hop header
  -D         insert a large destination header that fragments the packet
  -p srcport  set a specific UDP source port or Ping ID
  -s src6    set a specific IPv6 source address
  -m srcmac  set a specific MAC source address

Send an IPv4 packet to an IPv6 4to6 gateway. If a port is specified, a UDP packet is sent, otherwise an ICMPv4 ping.

~~~
