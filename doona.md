# doona command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


 Doona 1.0 by Wireghoul (www.justanotherhacker.com)

Usage:

 ./doona.pl -m [module] <options>

 -m <module>   = DICT/FINGER/FTP/HTTP/IMAP/IRC/LPD/NNTP/PJL/POP/PROXY/RTSP/SMTP/SOCKS4/SOCKS5/TFTP/WHOIS
 -c <int>      = Execute a health check after every <int> fuzz cases
 -t <target>   = Host to check (default: localhost)
 -p <port>     = Port to connect to (default: module specific standard port)
 -o <timeout>  = seconds to wait after each test (default: 2 seconds)
 -r <index>    = Resumes fuzzing at test case index
 -k            = Keep trying until server passes a health check
 -d            = Dump test case to stdout (use in combination with -r)
 -M <num>      = Exit after executing <num> number of fuzz cases
 -h            = Help (this text)
 use "./doona.pl -m [module] -h" for module specific option.

 Only -m is a mandatory switch.


~~~
