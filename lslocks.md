# lslocks command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 lslocks [options]

List local system locks.

Options:
 -J, --json             use JSON output format
 -n, --noheadings       don't print headings
 -o, --output <list>    define which output columns to use
 -p, --pid <pid>        display only locks held by this process
 -r, --raw              use the raw output format
 -u, --notruncate       don't truncate text in columns

 -h, --help     display this help and exit
 -V, --version  output version information and exit

Available columns (for --output):
     COMMAND  command of the process holding the lock
         PID  PID of the process holding the lock
        TYPE  kind of lock: FL_FLOCK or FL_POSIX.
        SIZE  size of the lock
        MODE  lock access mode
           M  mandatory state of the lock: 0 (none), 1 (set)
       START  relative byte offset of the lock
         END  ending offset of the lock
        PATH  path of the locked file
     BLOCKER  PID of the process blocking the lock

For more details see lslocks(8).

~~~
