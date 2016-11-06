# atk6-thcping6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-thcping6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-thcping6 [-Eafqx] [-e ethertype] [-H t:l:v] [-D t:l:v] [-F dst] [-e ethertype] [-L length] [-N nextheader] [-V version] [-t ttl] [-c class] [-l label] [-d size] [-S port|-U port|-T type -C code] interface src6 dst6 [srcmac [dstmac [data]]]

Options:
  -T number       ICMPv6 type to send (default: 128 = ping)
  -C number       ICMPv6 code to send (default: 0)
  -S port         use a TCP SYN packet on the defined port instead of ping
  -U port         use a UDP packet on the defined port instead of ping
  -n count        how often to send the packet (default: 1)
  -h              show more command line options (help!)
You can put an "x" into src6, srcmac and dstmac for an automatic value.

Craft a ICMPv6/TCP/UDP packet with special IPv6 or EH header options.
Returns -1 on error or no reply, 0 on normal reply or 1 on error reply.

~~~
