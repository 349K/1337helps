# sj-iptcpopt-probe command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: /usr/bin/sj-iptcpopt-probe options
This script is part of SniffJoke autotest

This script is invoked by sniffjoke-autotest and try the possibile
combination of IP/TCP header options for the testing 'location'

Is required a detailed test because different ISP will handle 
differently these options, considering a packet acceptable or not
by internal policy, router configuration and updating frequency

by hand this script should accept these argument:

OPTIONS:
   -h      show this message
   -w      working directory                                   (required)
            (eg: /tmp/home/, where sniffjoke-autotest is running)
   -u      testing URL                                         (required)
   -n      username to downgrade privileges
   -g      group to downgrade privileges
   -i      server IPv4 format 000.000.000.000                  (required)
   

~~~
