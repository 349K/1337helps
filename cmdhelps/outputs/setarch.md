# setarch command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 setarch <arch> [options] [<program> [<argument>...]]

Change the reported architecture and set personality flags.

Options:
 -B, --32bit              turns on ADDR_LIMIT_32BIT
 -F, --fdpic-funcptrs     makes function pointers point to descriptors
 -I, --short-inode        turns on SHORT_INODE
 -L, --addr-compat-layout changes the way virtual memory is allocated
 -R, --addr-no-randomize  disables randomization of the virtual address space
 -S, --whole-seconds      turns on WHOLE_SECONDS
 -T, --sticky-timeouts    turns on STICKY_TIMEOUTS
 -X, --read-implies-exec  turns on READ_IMPLIES_EXEC
 -Z, --mmap-page-zero     turns on MMAP_PAGE_ZERO
 -3, --3gb                limits the used address space to a maximum of 3 GB
     --4gb                ignored (for backward compatibility only)
     --uname-2.6          turns on UNAME26
 -v, --verbose            say what options are being switched on
     --list               list settable architectures, and exit

 -h, --help     display this help and exit
 -V, --version  output version information and exit

For more details see setarch(8).

~~~
