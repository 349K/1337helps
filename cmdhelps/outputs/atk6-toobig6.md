# atk6-toobig6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-toobig6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-toobig6 [-u] interface target-ip existing-ip mtu [hop-limit]

Implants the specified mtu on the target.
If the TTL of the target is not 64, then specify this as the last option.
Option -u will send the TooBig without the spoofed ping6 from existing-ip.

~~~
