# sc-hsm-tool command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: sc-hsm-tool [OPTIONS]
Options:
  -X, --initialize              Initialize token
  -C, --create-dkek-share <arg>
                                Create DKEK key share and save to <filename>
  -I, --import-dkek-share <arg>
                                Import DKEK key share <filename>
  -W, --wrap-key <arg>          Wrap key and save to <filename>
  -U, --unwrap-key <arg>        Unwrap key read from <filename>
  -s, --dkek-shares <arg>       Number of DKEK shares [No DKEK]
      --so-pin <arg>            Define security officer PIN (SO-PIN)
      --pin <arg>               Define user PIN
      --pin-retry <arg>         Define user PIN retry counter
      --password <arg>          Define password for DKEK share
      --pwd-shares-threshold <arg>
                                Define threshold for number of password shares required for reconstruction
      --pwd-shares-total <arg>  Define number of password shares
  -i, --key-reference <arg>     Key reference for key wrap/unwrap
  -l, --label <arg>             Token label for --initialize
  -f, --force                   Force replacement of key and certificate
  -r, --reader <arg>            Uses reader number <arg> [0]
  -w, --wait                    Wait for a card to be inserted
  -v, --verbose                 Verbose operation. Use several times to enable debug output.

~~~
