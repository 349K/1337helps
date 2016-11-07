# slabtop command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 slabtop [options]

Options:
 -d, --delay <secs>  delay updates
 -o, --once          only display once, then exit
 -s, --sort <char>   specify sort criteria by character (see below)

 -h, --help     display this help and exit
 -V, --version  output version information and exit

The following are valid sort criteria:
 a: sort by number of active objects
 b: sort by objects per slab
 c: sort by cache size
 l: sort by number of slabs
 v: sort by number of active slabs
 n: sort by name
 o: sort by number of objects (the default)
 p: sort by pages per slab
 s: sort by object size
 u: sort by cache utilization

For more details see slabtop(1).

~~~
