# snice command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 snice [new priority] [options] <expression>

Options:
 -f, --fast         fast mode (not implemented)
 -i, --interactive  interactive
 -l, --list         list all signal names
 -L, --table        list all signal names in a nice table
 -n, --no-action    do not actually kill processes; just print what would happen
 -v, --verbose      explain what is being done
 -w, --warnings     enable warnings (not implemented)

Expression can be: terminal, user, pid, command.
The options below may be used to ensure correct interpretation.
 -c, --command <command>  expression is a command name
 -p, --pid <pid>          expression is a process id number
 -t, --tty <tty>          expression is a terminal
 -u, --user <username>    expression is a username

Alternatively, expression can be:
 --ns <pid>               match the processes that belong to the same
                          namespace as <pid>
 --nslist <ns,...>        list which namespaces will be considered for
                          the --ns option; available namespaces are
:                          ipc, mnt, net, pid, user, uts


 -h, --help     display this help and exit
 -V, --version  output version information and exit

The default priority is +4. (snice +4 ...)
Priority numbers range from +20 (slowest) to -20 (fastest).
Negative priority numbers are restricted to administrative users.

For more details see snice(1).

~~~
