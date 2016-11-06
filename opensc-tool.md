# opensc-tool command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: opensc-tool [OPTIONS]
Options:
      --version                 Prints OpenSC package revision
  -i, --info                    Prints information about OpenSC
  -a, --atr                     Prints the ATR bytes of the card
      --serial                  Prints the card serial number
  -n, --name                    Identify the card and print its name
  -G, --get-conf-entry <arg>    Get configuration key, format: section:name:key
  -S, --set-conf-entry <arg>    Set configuration key, format: section:name:key:value
  -l, --list-readers            Lists readers
  -D, --list-drivers            Lists all installed card drivers
  -f, --list-files              Recursively lists files stored on card
  -s, --send-apdu <arg>         Sends an APDU in format AA:BB:CC:DD:EE:FF...
  -r, --reader <arg>            Uses reader number <arg> [0]
  -c, --card-driver <arg>       Forces the use of driver <arg> [auto-detect]
      --list-algorithms         Lists algorithms supported by card
  -w, --wait                    Wait for a card to be inserted
  -v, --verbose                 Verbose operation. Use several times to enable debug output.

~~~
