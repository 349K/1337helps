# impacket-netview command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Impacket v0.9.15 - Copyright 2002-2016 Core Security Technologies

usage: netview.py [-h] [-user USER] [-users USERS] [-target TARGET]
                  [-targets TARGETS] [-noloop] [-delay DELAY]
                  [-max-connections MAX_CONNECTIONS] [-debug]
                  [-hashes LMHASH:NTHASH] [-no-pass] [-k] [-aesKey hex key]
                  [-dc-ip ip address]
                  identity

positional arguments:
  identity              [domain/]username[:password]

optional arguments:
  -h, --help            show this help message and exit
  -user USER            Filter output by this user
  -users USERS          input file with list of users to filter to output for
  -target TARGET        target system to query info from. If not specified
                        script will run in domain mode.
  -targets TARGETS      input file with targets system to query info from (one
                        per line). If not specified script will run in domain
                        mode.
  -noloop               Stop after the first probe
  -delay DELAY          seconds delay between starting each batch probe
                        (default 10 seconds)
  -max-connections MAX_CONNECTIONS
                        Max amount of connections to keep opened (default
                        1000)
  -debug                Turn DEBUG output ON

authentication:
  -hashes LMHASH:NTHASH
                        NTLM hashes, format is LMHASH:NTHASH
  -no-pass              don't ask for password (useful for -k)
  -k                    Use Kerberos authentication. Grabs credentials from
                        ccache file (KRB5CCNAME) based on target parameters.
                        If valid credentials cannot be found, it will use the
                        ones specified in the command line
  -aesKey hex key       AES key to use for Kerberos Authentication (128 or 256
                        bits)
  -dc-ip ip address     IP Address of the domain controller. If ommited it use
                        the domain part (FQDN) specified in the target
                        parameter

~~~
