# atk6-kill_router6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-kill_router6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-kill_router6 [-HFD] interface router-address [srcmac [dstmac]]

Announce that a target a router going down to delete it from the routing tables.
If you supply a '*' as router-address, this tool will sniff the network for any
RA packet and immediately send the kill packet.
Option -H adds hop-by-hop, -F fragmentation header and -D dst header.

~~~
