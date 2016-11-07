# ipcs command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 ipcs [resource-option...] [output-option]
 ipcs -m|-q|-s -i <id>

Show information on IPC facilities.

Options:
 -i, --id <id>  print details on resource identified by <id>
 -h, --help     display this help and exit
 -V, --version  output version information and exit

Resource options:
 -m, --shmems      shared memory segments
 -q, --queues      message queues
 -s, --semaphores  semaphores
 -a, --all         all (default)

Output options:
 -t, --time        show attach, detach and change times
 -p, --pid         show PIDs of creator and last operator
 -c, --creator     show creator and owner
 -l, --limits      show resource limits
 -u, --summary     show status summary
     --human       show sizes in human-readable format
 -b, --bytes       show sizes in bytes

For more details see ipcs(1).

~~~
