# twistd command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: twistd [options]
Options:
      --savestats      save the Stats object rather than the text output of the
                       profiler.
  -o, --no_save        do not save state on shutdown
  -e, --encrypted      The specified tap/aos file is encrypted.
  -n, --nodaemon       don't daemonize, don't use default umask of 0077
      --originalname   Don't try to change the process name
      --syslog         Log to syslog, not to file
      --euid           Set only effective user-id rather than real user-id.
                       (This option has no effect unless the server is running
                       as root, in which case it means not to shed all
                       privileges after binding ports, retaining the option to
                       regain privileges in cases such as spawning processes.
                       Use with caution.)
  -l, --logfile=       log to a specified file, - for stdout
      --logger=        A fully-qualified name to a log observer factory to use
                       for the initial log observer.  Takes precedence over
                       --logfile and --syslog (when available).
  -p, --profile=       Run in profile mode, dumping results to specified file.
      --profiler=      Name of the profiler to use (profile, cprofile).
                       [default: cprofile]
  -f, --file=          read the given .tap file [default: twistd.tap]
  -y, --python=        read an application from within a Python file (implies
                       -o)
  -s, --source=        Read an application from a .tas file (AOT format).
  -d, --rundir=        Change to a supplied directory before running [default:
                       .]
      --prefix=        use the given prefix when syslogging [default: twisted]
      --pidfile=       Name of the pidfile [default: twistd.pid]
      --chroot=        Chroot to a supplied directory before running
  -u, --uid=           The uid to run as.
  -g, --gid=           The gid to run as.
      --umask=         The (octal) file creation mask to apply.
      --help-reactors  Display a list of possibly available reactor names.
      --version        Print version information and exit.
      --spew           Print an insanely verbose log of everything that happens.
                       Useful when debugging freezes or locks in complex code.
  -b, --debug          Run the application in the Python Debugger (implies
                       nodaemon),         sending SIGUSR2 will drop into
                       debugger
  -r, --reactor=       Which reactor to use (see --help-reactors for a list of
                       possibilities)
      --help           Display this help and exit.

twistd reads a twisted.application.service.Application out of a file and runs
it.
Commands:
    conch            A Conch SSH service.
    dns              A domain name server.
    ftp              An FTP server.
    inetd            An inetd(8) replacement.
    mail             An email service
    manhole          An interactive remote debugger service accessible via
                     telnet and ssh and providing syntax coloring and basic line
                     editing functionality.
    news             A news server.
    portforward      A simple port-forwarder.
    procmon          A process watchdog / supervisor
    socks            A SOCKSv4 proxy service.
    web              A general-purpose web server which can serve from a
                     filesystem or application resource.
    words            A modern words server
    xmpp-router      An XMPP Router server


~~~
