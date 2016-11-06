# systemd-resolve command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


systemd-resolve [OPTIONS...] HOSTNAME|ADDRESS...
systemd-resolve [OPTIONS...] --service [[NAME] TYPE] DOMAIN
systemd-resolve [OPTIONS...] --openpgp EMAIL@DOMAIN...
systemd-resolve [OPTIONS...] --statistics
systemd-resolve [OPTIONS...] --reset-statistics

Resolve domain names, IPv4 and IPv6 addresses, DNS resource records, and services.

  -h --help                 Show this help
     --version              Show package version
     --no-pager             Do not pipe output into a pager
  -4                        Resolve IPv4 addresses
  -6                        Resolve IPv6 addresses
  -i --interface=INTERFACE  Look on interface
  -p --protocol=PROTO|help  Look via protocol
  -t --type=TYPE|help       Query RR with DNS type
  -c --class=CLASS|help     Query RR with DNS class
     --service              Resolve service (SRV)
     --service-address=BOOL Resolve address for services (default: yes)
     --service-txt=BOOL     Resolve TXT records for services (default: yes)
     --openpgp              Query OpenPGP public key
     --tlsa                 Query TLS public key
     --cname=BOOL           Follow CNAME redirects (default: yes)
     --search=BOOL          Use search domains for single-label names
                                                              (default: yes)
     --raw[=payload|packet] Dump the answer as binary data
     --legend=BOOL          Print headers and additional info (default: yes)
     --statistics           Show resolver statistics
     --reset-statistics     Reset resolver statistics
     --status               Show link and server status
     --flush-caches         Flush all local DNS caches

~~~
