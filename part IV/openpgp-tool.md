# openpgp-tool command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: openpgp-tool [OPTIONS]
Options:
  -r, --reader <arg>            Use reader number <arg> [0]
  -w, --wait                    Wait for card insertion
  -x, --exec <arg>              Execute program <arg> with data in env vars
      --raw                     Print values in raw format
      --pretty                  Print values in pretty format
  -U, --user-info               Show card holder information
  -G, --gen-key <arg>           Generate key
  -L, --key-length <arg>        Key length (default 2048)
  -h, --help                    Print this help message
  -v, --verbose                 Verbose operation. Use several times to enable debug output.
  -V, --version                 Show version number
  -E, --erase                   Erase (reset) the card
      --verify <arg>            Verify PIN (CHV1, CHV2, CHV3...)
      --pin <arg>               PIN string
      --del-key <arg>           Delete key (1, 2, 3 or all)
  -d, --do <arg>                Dump private data object number <arg> (i.e. PRIVATE-DO-<arg>)

~~~
