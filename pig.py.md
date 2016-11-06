# pig.py command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


enhanced DHCP exhaustion attack.

Doc:
    http://github.com/kamorin/DHCPig


Usage:
    pig.py [-h -v -6 -1 -s -f -t -a -i -o -l -x -y -z -g -r -n -c ] <interface>
  
Options:
    -h, --help                     <-- you are here :)
    -v, --verbosity                ...  0 ... no         (3)
                                        1 ... minimal
                                       10 ... default
                                       99 ... debug
                                       
    -6, --ipv6                     ... DHCPv6 (off, DHCPv4 by default)
    -1, --v6-rapid-commit          ... enable RapidCommit (2way ip assignment instead of 4way) (off)
    
    -s, --client-src               ... a list of client macs 00:11:22:33:44:55,00:11:22:33:44:56 (Default: <random>)
    -O, --request-options          ... option-codes to request e.g. 21,22,23 or 12,14-19,23 (Default: 0-80)
    
    -f, --fuzz                     ... randomly fuzz packets (off)

    -t, --threads                  ... number of sending threads (1)
    
    -a, --show-arp                 ... detect/print arp who_has (off)
    -i, --show-icmp                ... detect/print icmps requests (off)
    -o, --show-options             ... print lease infos (off)
    -l, --show-lease-confirm       ... detect/print dhcp replies (off)
    
    -g, --neighbors-attack-garp    ... knock off network segment using gratious arps (off)
    -r, --neighbors-attack-release ... release all neighbor ips (off)
    -n, --neighbors-scan-arp       ... arp neighbor scan (off)
    
    -x, --timeout-threads          ... thread spawn timer (0.4)
    -y, --timeout-dos              ... DOS timeout (8) (wait time to mass grat.arp)
    -z, --timeout-dhcprequest      ... dhcp request timeout (2)
    
    -c, --color                    ... enable color output (off)


~~~
