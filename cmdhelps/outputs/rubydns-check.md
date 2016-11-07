# rubydns-check command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: rubydns-check [options]
This script is designed to test and check DNS servers.
  -s, --server ns.my.domain.       The DNS server to query.
  -d, --domain my.domain.          The DNS zone to transfer/test.
  -f, --fetch output.yml           Pull down a list of hosts. Filters TXT and HINFO records. DNS transfers must be enabled.
  -c, --check input.yml            Check that the DNS server returns results as specified by the file.
  -q, --query input.yml            Query the remote DNS server with all hostnames in the given file, and checks the IP addresses are consistent.
  -p, --ping input.yml             Ping all hosts to check if they are available or not.
  -r, --reverse input.yml          Check that all address records have appropriate reverse entries.

Help and Copyright information
      --copy                       Display copyright information
  -h, --help                       Show this help message.

~~~
