# impacket-samrdump command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Impacket v0.9.15 - Copyright 2002-2016 Core Security Technologies

usage: samrdump.py [-h] [-debug] [-hashes LMHASH:NTHASH] [-no-pass] [-k]
                   [-aesKey hex key] [-dc-ip ip address]
                   target [{445/SMB,139/SMB}]

This script downloads the list of users for the target system.

positional arguments:
  target                [[domain/]username[:password]@]<targetName or address>
  {445/SMB,139/SMB}     transport protocol (default 445/SMB)

optional arguments:
  -h, --help            show this help message and exit
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
