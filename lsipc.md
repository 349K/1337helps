# lsipc command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 lsipc [options]

Show information on IPC facilities.

Resource options:
 -m, --shmems      shared memory segments
 -q, --queues      message queues
 -s, --semaphores  semaphores
 -g, --global      info about system-wide usage (may be used with -m, -q and -s)
 -i, --id <id>     print details on resource identified by <id>

Options:
     --noheadings         don't print headings
     --notruncate         don't truncate output
     --time-format=<type> display dates in short, full or iso format
 -b, --bytes              print SIZE in bytes rather than in human readable format
 -c, --creator            show creator and owner
 -e, --export             display in an export-able output format
 -J, --json               use the JSON output format
 -n, --newline            display each piece of information on a new line
 -l, --list               force list output format (for example with --id)
 -o, --output[=<list>]    define the columns to output
 -P, --numeric-perms      print numeric permissions (PERMS column)
 -r, --raw                display in raw mode
 -t, --time               show attach, detach and change times

 -h, --help     display this help and exit
 -V, --version  output version information and exit

Generic columns:
            KEY  Resource key
             ID  Resource ID
          OWNER  Owner's username or UID
          PERMS  Permissions
           CUID  Creator UID
          CUSER  Creator user
           CGID  Creator GID
         CGROUP  Creator group
            UID  User ID
           USER  User name
            GID  Group ID
          GROUP  Group name
          CTIME  Time of the last change

Shared-memory columns (--shmems):
           SIZE  Segment size
         NATTCH  Number of attached processes
         STATUS  Status
         ATTACH  Attach time
         DETACH  Detach time
        COMMAND  Creator command line
           CPID  PID of the creator
           LPID  PID of last user

Message-queue columns (--queues):
      USEDBYTES  Bytes used
           MSGS  Number of messages
           SEND  Time of last msg sent
           RECV  Time of last msg received
          LSPID  PID of the last msg sender
          LRPID  PID of the last msg receiver

Semaphore columns (--semaphores):
          NSEMS  Number of semaphores
          OTIME  Time of the last operation

Summary columns (--global):
       RESOURCE  Resource name
    DESCRIPTION  Resource description
          LIMIT  System-wide limit
           USED  Currently used
           USE%  Currently use percentage

For more details see lsipc(1).

~~~
