# piv-tool command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: piv-tool [OPTIONS]
Options:
      --serial                  Print the card serial number
  -n, --name                    Identify the card and print its name
  -A, --admin <arg>             Authenticate using default 3DES key
  -G, --genkey <arg>            Generate key <ref>:<alg> 9A:06 on card, and output pubkey
  -O, --object <arg>            Load an object <containerID> containerID as defined in 800-73 without leading 0x
  -C, --cert <arg>              Load a cert <ref> where <ref> is 9A,9C,9D or 9E
  -Z, --compresscert <arg>      Load a cert that has been gzipped <ref>
  -o, --out <arg>               Output file for cert or key
  -i, --in <arg>                Input file for cert
  -s, --send-apdu <arg>         Sends an APDU in format AA:BB:CC:DD:EE:FF...
  -r, --reader <arg>            Uses reader number <arg> [0]
  -c, --card-driver <arg>       Forces the use of driver <arg> [auto-detect]
  -w, --wait                    Wait for a card to be inserted
  -v, --verbose                 Verbose operation. Use several times to enable debug output.

~~~
