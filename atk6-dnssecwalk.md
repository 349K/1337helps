# atk6-dnssecwalk command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-dnssecwalk v1.2 (c) 2014 by Marc Heuse <mh@mh-sec.de> http://www.mh-sec.de

Syntax: atk6-dnssecwalk [-e46] dns-server domain

Options:
 -e  ensure that the domain is present in found addresses, quit otherwise
 -4  resolve found entries to IPv4 addresses
 -6  resolve found entries to IPv6 addresses

Perform DNSSEC NSEC walking.

Example: atk6-dnssecwalk dns.test.com test.com

~~~
