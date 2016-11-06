# atk6-trace6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-trace6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-trace6 [-abdtu] [-s src6] interface targetaddress [port]

Options:
  -a       insert a hop-by-hop header with router alert option.
  -D       insert a destination extension header
  -E       insert a destination extension header with an invalid option
  -F       insert a one-shot fragmentation header
  -b       instead of an ICMP6 Ping, use TooBig (you will not see the target)
  -B       instead of an ICMP6 Ping, use PingReply (you will not see the target)
  -d       resolves the IPv6 addresses to DNS.
  -t       enables tunnel detection
  -u       use UDP instead of TCP if a port is supplied
  -s src6  specifies the source IPv6 address
Maximum hop reach: 31

A basic but very fast traceroute6 program.
If no port is specified, ICMP6 Ping requests are used, otherwise TCP SYN
packets to the specified port. Options D, E and F can be use multiple times.

~~~
