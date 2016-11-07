# winedbg-stable command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
   winedbg <cmdline>       launch process <cmdline> (as if you were starting
                           it with wine) and run WineDbg on it
   winedbg <num>           attach to running process of wpid <num> and run
                           WineDbg on it
   winedbg --gdb <cmdline> launch process <cmdline> (as if you were starting
                           wine) and run gdb (proxied) on it
   winedbg --gdb <num>     attach to running process of wpid <num> and run
                           gdb (proxied) on it
   winedbg <file.mdmp>     reload the minidump <file.mdmp> into memory and run
                           WineDbg on it
   winedbg --help          prints advanced options

~~~
