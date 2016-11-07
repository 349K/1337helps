# rafind2 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: rafind2 [-Xnzhv] [-b sz] [-f/t from/to] [-[m|s|S|e] str] [-x hex] file ..
 -h         show this help
 -v         print version and exit
 -b [size]  set block size
 -f [from]  start searching from address 'from'
 -t [to]    stop search at address 'to'
 -n         do not stop on read errors
 -s [str]   search for a specific string (can be used multiple times)
 -S [str]   search for a specific wide string (can be used multiple times)
 -x [hex]   search for hexpair string (909090) (can be used multiple times)
 -e [regex] search for regular expression string matches
 -m [str]   set a binary mask to be applied on keywords
 -z         search for zero-terminated strings
 -r         print using radare commands
 -X         show hexdump of search results
 -Z         show zero-terminated strings of search results

~~~
