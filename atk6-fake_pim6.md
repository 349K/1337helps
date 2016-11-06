# atk6-fake_pim6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-fake_pim6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax:
  atk6-fake_pim6 [-t ttl] [-s src6] [-d dst6] interface hello [dr_priority]
  atk6-fake_pim6 [-t ttl] [-s src6] [-d dst6] interface join|prune neighbor6 multicast6 target6

The hello command takes optionally the DR priority (default: 0).
The join and prune commands need the multicast group to modify, the target
address that joins or leavs and the neighbor PIM router
Use -s to spoof the source ip6, -d to send to another address than ff02::d,
and -t to set a different TTL (default: 1)

~~~
