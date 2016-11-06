# westcos-tool command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: westcos-tool [OPTIONS]
Options:
  -r, --reader <arg>            Uses reader number <arg> [0]
  -w, --wait                    Wait for card insertion
  -g, --generate-key            Generate key 1536 default
  -o, --overwrite-key           Overwrite key if already exist
  -l, --key-length <arg>        Key length <arg> [512,1024,1536]
  -i, --install-pin             Install pin
  -x, --pin-value <arg>         Pin value <arg>
  -y, --puk-value <arg>         Puk value <arg>
  -n, --change-pin              Change pin (new pin in puk value)
  -u, --unblock-pin             Unblock pin
  -t, --certificate <arg>       Write certificate <arg> (in pem format)
  -f, --finalize                Finalize card(!!! MANDATORY FOR SECURITY !!!)
  -j, --read-file <arg>         Read file <arg>
  -k, --write-file <arg>        Write file <arg> (ex 0002 write file 0002 to 0002)
  -h, --help                    This message
  -v, --verbose                 Verbose operation. Use several times to enable debug output.

~~~
