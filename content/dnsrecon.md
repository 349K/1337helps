# dnsrecon command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Version: 0.8.10
Usage: dnsrecon.py <options>

Options:
   -h, --help                   Show this help message and exit.
   -d, --domain      <domain>   Target domain.
   -r, --range       <range>    IP range for reverse lookup brute force in formats (first-last) or in (range/bitmask).
   -n, --name_server <name>     Domain server to use. If none is given, the SOA of the target will be used.
   -D, --dictionary  <file>     Dictionary file of subdomain and hostnames to use for brute force.
   -f                           Filter out of brute force domain lookup, records that resolve to the wildcard defined
                                IP address when saving records.
   -t, --type        <types>    Type of enumeration to perform:
                                std       SOA, NS, A, AAAA, MX and SRV if AXRF on the NS servers fail.
                                rvl       Reverse lookup of a given CIDR or IP range.
                                brt       Brute force domains and hosts using a given dictionary.
                                srv       SRV records.
                                axfr      Test all NS servers for a zone transfer.
                                goo       Perform Google search for subdomains and hosts.
                                snoop     Perform cache snooping against all NS servers for a given domain, testing
                                          all with file containing the domains, file given with -D option.
                                tld       Remove the TLD of given domain and test against all TLDs registered in IANA.
                                zonewalk  Perform a DNSSEC zone walk using NSEC records.
   -a                           Perform AXFR with standard enumeration.
   -s                           Perform a reverse lookup of IPv4 ranges in the SPF record with standard enumeration.
   -g                           Perform Google enumeration with standard enumeration.
   -w                           Perform deep whois record analysis and reverse lookup of IP ranges found through
                                Whois when doing a standard enumeration.
   -z                           Performs a DNSSEC zone walk with standard enumeration.
   --threads         <number>   Number of threads to use in reverse lookups, forward lookups, brute force and SRV
                                record enumeration.
   --lifetime        <number>   Time to wait for a server to response to a query.
   --db              <file>     SQLite 3 file to save found records.
   --xml             <file>     XML file to save found records.
   --iw                         Continue brute forcing a domain even if a wildcard records are discovered.
   -c, --csv         <file>     Comma separated value file.
   -j, --json        <file>     JSON file.
   -v                           Show attempts in the brute force modes.

~~~
