# impacket-secretsdump command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Impacket v0.9.15 - Copyright 2002-2016 Core Security Technologies

usage: secretsdump.py [-h] [-debug] [-system SYSTEM] [-security SECURITY]
                      [-sam SAM] [-ntds NTDS] [-resumefile RESUMEFILE]
                      [-outputfile OUTPUTFILE] [-use-vss]
                      [-just-dc-user USERNAME] [-just-dc] [-just-dc-ntlm]
                      [-pwd-last-set] [-history] [-hashes LMHASH:NTHASH]
                      [-no-pass] [-k] [-aesKey hex key] [-dc-ip ip address]
                      target

Performs various techniques to dump secrets from the remote machine without
executing any agent there.

positional arguments:
  target                [[domain/]username[:password]@]<targetName or address>
                        or LOCAL (if you want to parse local files)

optional arguments:
  -h, --help            show this help message and exit
  -debug                Turn DEBUG output ON
  -system SYSTEM        SYSTEM hive to parse
  -security SECURITY    SECURITY hive to parse
  -sam SAM              SAM hive to parse
  -ntds NTDS            NTDS.DIT file to parse
  -resumefile RESUMEFILE
                        resume file name to resume NTDS.DIT session dump (only
                        available to DRSUAPI approach). This file will also be
                        used to keep updating the session's state
  -outputfile OUTPUTFILE
                        base output filename. Extensions will be added for
                        sam, secrets, cached and ntds
  -use-vss              Use the VSS method insead of default DRSUAPI

display options:
  -just-dc-user USERNAME
                        Extract only NTDS.DIT data for the user specified.
                        Only available for DRSUAPI approach. Implies also
                        -just-dc switch
  -just-dc              Extract only NTDS.DIT data (NTLM hashes and Kerberos
                        keys)
  -just-dc-ntlm         Extract only NTDS.DIT data (NTLM hashes only)
  -pwd-last-set         Shows pwdLastSet attribute for each NTDS.DIT account.
                        Doesn't apply to -outputfile data
  -history              Dump password history

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
