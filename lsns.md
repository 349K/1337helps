# lsns command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 lsns [options] [<namespace>]

List system namespaces.

Options:
 -J, --json             use JSON output format
 -l, --list             use list format output
 -n, --noheadings       don't print headings
 -o, --output <list>    define which output columns to use
 -p, --task <pid>       print process namespaces
 -r, --raw              use the raw output format
 -u, --notruncate       don't truncate text in columns
 -t, --type <name>      namespace type (mnt, net, ipc, user, pid, uts)

 -h, --help     display this help and exit
 -V, --version  output version information and exit

Available columns (for --output):
          NS  namespace identifier (inode number)
        TYPE  kind of namespace
        PATH  path to the namespace
      NPROCS  number of processes in the namespace
         PID  lowest PID in the namespace
        PPID  PPID of the PID
     COMMAND  command line of the PID
         UID  UID of the PID
        USER  username of the PID

For more details see lsns(8).

~~~
