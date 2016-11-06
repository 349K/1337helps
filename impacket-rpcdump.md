# impacket-rpcdump command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Impacket v0.9.15 - Copyright 2002-2016 Core Security Technologies

usage: rpcdump.py [-h] [-debug] [-hashes LMHASH:NTHASH]
                  target [{445/SMB,135/TCP,139/SMB}]

Dumps the remote RPC enpoints information.

positional arguments:
  target                [[domain/]username[:password]@]<targetName or address>
  {445/SMB,135/TCP,139/SMB}
                        transport protocol (default 135/TCP)

optional arguments:
  -h, --help            show this help message and exit
  -debug                Turn DEBUG output ON

authentication:
  -hashes LMHASH:NTHASH
                        NTLM hashes, format is LMHASH:NTHASH

~~~
