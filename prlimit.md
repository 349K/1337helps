# prlimit command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 prlimit [options] [-p PID]
 prlimit [options] COMMAND

Show or change the resource limits of a process.

General Options:
 -p, --pid <pid>        process id
 -o, --output <list>    define which output columns to use
     --noheadings       don't print headings
     --raw              use the raw output format
     --verbose          verbose output
 -h, --help             display this help and exit
 -V, --version          output version information and exit

Resources Options:
 -c, --core             maximum size of core files created
 -d, --data             maximum size of a process's data segment
 -e, --nice             maximum nice priority allowed to raise
 -f, --fsize            maximum size of files written by the process
 -i, --sigpending       maximum number of pending signals
 -l, --memlock          maximum size a process may lock into memory
 -m, --rss              maximum resident set size
 -n, --nofile           maximum number of open files
 -q, --msgqueue         maximum bytes in POSIX message queues
 -r, --rtprio           maximum real-time scheduling priority
 -s, --stack            maximum stack size
 -t, --cpu              maximum amount of CPU time in seconds
 -u, --nproc            maximum number of user processes
 -v, --as               size of virtual memory
 -x, --locks            maximum number of file locks
 -y, --rttime           CPU time in microseconds a process scheduled
                        under real-time scheduling

Available columns (for --output):
 DESCRIPTION  resource description
    RESOURCE  resource name
        SOFT  soft limit
        HARD  hard limit (ceiling)
       UNITS  units

For more details see prlimit(1).

~~~
