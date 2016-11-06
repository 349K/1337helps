# atk6-covert_send6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-covert_send6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-covert_send6 [-m mtu] [-k key] [-s resend] interface target file [port]

Options:
  -m mtu     specifies the maximum MTU (default: interface MTU, min: 1000)
  -k key     encrypt the content with Blowfish-160
  -s resend  send each packet RESEND number of times, default: 1

Sends the content of FILE covertly to the target, And its POC - don't except
too much sophistication - its just put into the destination header.

~~~
