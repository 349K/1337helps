# atk6-redir6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-redir6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-redir6 interface victim-ip target-ip original-router new-router [new-router-mac] [hop-limit]

Implant a route into victim-ip, which redirects all traffic to target-ip to
new-ip. You must know the router which would handle the route.
If the new-router-mac does not exist, this results in a DOS.
If the TTL of the target is not 64, then specify this is the last option.

~~~
