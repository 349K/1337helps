# lscpu command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 lscpu [options]

Display information about the CPU architecture.

Options:
 -a, --all               print both online and offline CPUs (default for -e)
 -b, --online            print online CPUs only (default for -p)
 -c, --offline           print offline CPUs only
 -e, --extended[=<list>] print out an extended readable format
 -p, --parse[=<list>]    print out a parsable format
 -s, --sysroot <dir>     use specified directory as system root
 -x, --hex               print hexadecimal masks rather than lists of CPUs

 -h, --help     display this help and exit
 -V, --version  output version information and exit

Available columns:
           CPU  logical CPU number
          CORE  logical core number
        SOCKET  logical socket number
          NODE  logical NUMA node number
          BOOK  logical book number
         CACHE  shows how caches are shared between CPUs
  POLARIZATION  CPU dispatching mode on virtual hardware
       ADDRESS  physical address of a CPU
    CONFIGURED  shows if the hypervisor has allocated the CPU
        ONLINE  shows if Linux currently makes use of the CPU
        MAXMHZ  shows the maximum MHz of the CPU
        MINMHZ  shows the minimum MHz of the CPU

For more details see lscpu(1).

~~~
