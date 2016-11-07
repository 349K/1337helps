# cardos-tool command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

NB! This tool is only for Siemens CardOS based cards!

Usage: cardos-tool [OPTIONS]
Options:
  -h, --help                    Print this help message
  -i, --info                    Print information about this card
  -f, --format                  Format this card erasing all content
  -s, --startkey <arg>          Specify startkey for format
  -S, --change-startkey <arg>   Change Startkey with given APDU command
  -r, --reader <arg>            Uses reader number <arg> [0]
  -c, --card-driver <arg>       Forces the use of driver <arg> [auto-detect]
  -w, --wait                    Wait for a card to be inserted
  -v, --verbose                 Verbose operation. Use several times to enable debug output.

~~~
