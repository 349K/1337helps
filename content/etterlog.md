# etterlog command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


[1metterlog 0.8.2[0m copyright 2001-2015 Ettercap Development Team


Usage: etterlog [OPTIONS] logfile

General Options:
  -a, --analyze               analyze a log file and return useful infos
  -c, --connections           display the table of connections
  -f, --filter <TARGET>       print packets only from this target
  -t, --proto <proto>         display only this proto (default is all)
  -F, --filcon <CONN>         print packets only from this connection 
  -s, --only-source           print packets only from the source
  -d, --only-dest             print packets only from the destination
  -r, --reverse               reverse the target/connection matching
  -n, --no-headers            skip header information between packets
  -m, --show-mac              show mac addresses in the headers
  -k, --color                 colorize the output
  -l, --only-local            show only local hosts parsing info files
  -L, --only-remote           show only remote hosts parsing info files

Search Options:
  -e, --regex <regex>         display only packets that match the regex
  -u, --user <user>           search for info about the user <user>
  -p, --passwords             print only accounts information
  -i, --show-client           show client address in the password profiles
  -I, --client <ip>           search for pass from a specific client

Editing Options:
  -C, --concat                concatenate more files into one single file
  -o, --outfile <file>        the file used as output for concatenation
  -D, --decode                used to extract files from connections

Visualization Method:
  -B, --binary                print packets as they are
  -X, --hex                   print packets in hex mode
  -A, --ascii                 print packets in ascii mode (default)
  -T, --text                  print packets in text mode
  -E, --ebcdic                print packets in ebcdic mode
  -H, --html                  print packets in html mode
  -U, --utf8 <encoding>       print packets in uft-8 using the <encoding>
  -Z, --zero                  do not print packets, only headers
  -x, --xml                   print host infos in xml format

Standard Options:
  -v, --version               prints the version and exit
  -h, --help                  this help screen



~~~
