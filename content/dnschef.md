# dnschef command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dnschef.py [options]:
          _                _          __  
         | | version 0.2  | |        / _| 
       __| |_ __  ___  ___| |__   ___| |_ 
      / _` | '_ \/ __|/ __| '_ \ / _ \  _|
     | (_| | | | \__ \ (__| | | |  __/ |  
      \__,_|_| |_|___/\___|_| |_|\___|_|  
                   iphelix@thesprawl.org  


DNSChef is a highly configurable DNS Proxy for Penetration Testers and Malware
Analysts. It is capable of fine configuration of which DNS replies to modify
or to simply proxy with real responses. In order to take advantage of the tool
you must either manually configure or poison DNS server entry to point to
DNSChef. The tool requires root privileges to run on privileged ports.

Options:
  -h, --help            show this help message and exit
  --fakedomains=thesprawl.org,google.com
                        A comma separated list of domain names which will be
                        resolved to FAKE values specified in the the above
                        parameters. All other domain names will be resolved to
                        their true values.
  --truedomains=thesprawl.org,google.com
                        A comma separated list of domain names which will be
                        resolved to their TRUE values. All other domain names
                        will be resolved to fake values specified in the above
                        parameters.

  Fake DNS records::
    --fakeip=192.0.2.1  IP address to use for matching DNS queries. If you use
                        this parameter without specifying domain names, then
                        all 'A' queries will be spoofed. Consider using --file
                        argument if you need to define more than one IP
                        address.
    --fakeipv6=2001:db8::1
                        IPv6 address to use for matching DNS queries. If you
                        use this parameter without specifying domain names,
                        then all 'AAAA' queries will be spoofed. Consider
                        using --file argument if you need to define more than
                        one IPv6 address.
    --fakemail=mail.fake.com
                        MX name to use for matching DNS queries. If you use
                        this parameter without specifying domain names, then
                        all 'MX' queries will be spoofed. Consider using
                        --file argument if you need to define more than one MX
                        record.
    --fakealias=www.fake.com
                        CNAME name to use for matching DNS queries. If you use
                        this parameter without specifying domain names, then
                        all 'CNAME' queries will be spoofed. Consider using
                        --file argument if you need to define more than one
                        CNAME record.
    --fakens=ns.fake.com
                        NS name to use for matching DNS queries. If you use
                        this parameter without specifying domain names, then
                        all 'NS' queries will be spoofed. Consider using
                        --file argument if you need to define more than one NS
                        record.
    --file=FILE         Specify a file containing a list of DOMAIN=IP pairs
                        (one pair per line) used for DNS responses. For
                        example: google.com=1.1.1.1 will force all queries to
                        'google.com' to be resolved to '1.1.1.1'. IPv6
                        addresses will be automatically detected. You can be
                        even more specific by combining --file with other
                        arguments. However, data obtained from the file will
                        take precedence over others.

  Optional runtime parameters.:
    --nameservers=8.8.8.8#53 or 2001:4860:4860::8888
                        A comma separated list of alternative DNS servers to
                        use with proxied requests. Nameservers can have either
                        IP or IP#PORT format. A randomly selected server from
                        the list will be used for proxy requests when provided
                        with multiple servers. By default, the tool uses
                        Google's public DNS server 8.8.8.8 when running in
                        IPv4 mode and 2001:4860:4860::8888 when running in
                        IPv6 mode.
    -i 127.0.0.1 or ::1, --interface=127.0.0.1 or ::1
                        Define an interface to use for the DNS listener. By
                        default, the tool uses 127.0.0.1 for IPv4 mode and ::1
                        for IPv6 mode.
    -t, --tcp           Use TCP DNS proxy instead of the default UDP.
    -6, --ipv6          Run in IPv6 mode.
    -p 53, --port=53    Port number to listen for DNS requests.
    -q, --quiet         Don't show headers.

~~~
