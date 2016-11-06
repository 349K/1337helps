# atk6-denial6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-denial6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-denial6 interface destination test-case-number

Performs various denial of service attacks on a target
If a system is vulnerable, it can crash or be under heavy load, so be careful!
The following test cases are currently implemented:
  1 : large hop-by-hop header with router-alert and filled with unknown options
  2 : large destination header filled with unknown options
  3 : hop-by-hop header with router alert option plus 180 headers
  4 : hop-by-hop header with router alert option plus 178 headers + ping
  5 : AH header + ping
  6 : first fragments of a ping with a hop-by-hop header with router alert
  7 : large hop-by-hop header filled with unknown options (no router alert)


~~~
