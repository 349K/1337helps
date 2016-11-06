# atk6-ndpexhaust26 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-ndpexhaust26 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-ndpexhaust26 [-acpPTUrR] [-s sourceip6] interface target-network

Options:
 -a      add a hop-by-hop header with router alert
 -c      do not calculate the checksum to save time
 -p      send ICMPv6 Echo Requests
 -P      send ICMPv6 Echo Reply
 -T      send ICMPv6 Time-to-live-exeeded
 -U      send ICMPv6 Unreachable (no route)
 -r      randomize the source from your /64 prefix
 -R      randomize the source fully
 -s sourceip6  use this as source IPv6 address

Flood the target /64 network with ICMPv6 TooBig error messages.
This tool version is manyfold more effective than ndpexhaust6.

~~~
