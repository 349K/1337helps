# atk6-fake_mld26 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-fake_mld26 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-fake_mld26 [-l] interface add|delete|query [multicast-address [target-address-to-subscribe-from [ttl [own-ip [own-mac-address [destination-mac-address]]]]]]

This uses the MLDv2 protocol. Only a subset of what the protocol is able to
do is possible to implement via a command line. Code it if you need something.
Ad(d)vertise or delete yourself - or anyone you want - in a multicast group of your choice
Query ask on the network who is listening to multicast addresses
Use -l to loop and send (in 5s intervals) until Control-C is pressed.

~~~
