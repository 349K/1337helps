# atk6-dnsdict6 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


atk6-dnsdict6 v2.7 (c) 2014 by van Hauser / THC <vh@thc.org> www.thc.org

Syntax: atk6-dnsdict6 [-d4] [-s|-m|-l|-x|-u] [-t THREADS] [-D] domain [dictionary-file]

Enumerates a domain for DNS entries, it uses a dictionary file if supplied
or a built-in list otherwise. This tool is based on dnsmap by gnucitizen.org.

Options:
 -4      do also dump IPv4 addresses
 -t NO   specify the number of threads to use (default: 8, max: 32).
 -D      dump the selected built-in wordlist, no scanning.
 -d      display IPv6 information on NS and MX DNS domain information.
 -e      ignore no NS for domain errors
 -S      perform SRV service name guessing
 -[smlxu] choose the dictionary size by -s(mall=100), -m(edium=1419) (DEFAULT)
           -l(arge=2601), -x(treme=5886) or -u(ber=16724)


~~~
