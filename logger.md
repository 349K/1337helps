# logger command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 logger [options] [<message>]

Enter messages into the system log.

Options:
 -i                       log the logger command's PID
     --id[=<id>]          log the given <id>, or otherwise the PID
 -f, --file <file>        log the contents of this file
 -e, --skip-empty         do not log empty lines when processing files
     --no-act             do everything except the write the log
 -p, --priority <prio>    mark given message with this priority
     --octet-count        use rfc6587 octet counting
     --prio-prefix        look for a prefix on every line read from stdin
 -s, --stderr             output message to standard error as well
 -S, --size <size>        maximum size for a single message
 -t, --tag <tag>          mark every line with this tag
 -n, --server <name>      write to this remote syslog server
 -P, --port <port>        use this port for UDP or TCP connection
 -T, --tcp                use TCP only
 -d, --udp                use UDP only
     --rfc3164            use the obsolete BSD syslog protocol
     --rfc5424[=<snip>]   use the syslog protocol (the default for remote);
                            <snip> can be notime, or notq, and/or nohost
     --sd-id <id>         rfc5424 structured data ID
     --sd-param <data>    rfc5424 structured data name=value
     --msgid <msgid>      set rfc5424 message id field
 -u, --socket <socket>    write to this Unix socket
     --socket-errors[=<on|off|auto>]
                          print connection errors when using Unix sockets
     --journald[=<file>]  write journald entry

 -h, --help     display this help and exit
 -V, --version  output version information and exit

For more details see logger(1).

~~~
