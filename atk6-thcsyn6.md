# atk6-thcsyn6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-thcsyn6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-thcsyn6 [-AcDrRS] [-m dstmac] [-p port] [-s sourceip6] interface target port

Options:
 -a      add hop-by-hop header with router alert
 -d      add destination header (can be set up to 150 times)
 -A      send TCP-ACK packets
 -S      send TCP-SYN-ACK packets
 -r      randomize the source from your /64 prefix
 -R      randomize the source fully
 -D      randomize the destination (treat as /64)
 -m dstmac     use this destination mac address
 -s sourceip6  use this as source IPv6 address
 -p port       use fixed source port

Flood the target port with TCP-SYN packets. If you supply "x" as port, it
is randomized.

~~~
