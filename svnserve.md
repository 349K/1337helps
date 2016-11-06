# svnserve command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: svnserve [-d | -i | -t | -X] [options]
Subversion repository server.
Type 'svnserve --version' to see the program version.

Valid options:
  -d [--daemon]            : daemon mode
  -i [--inetd]             : inetd mode
  -t [--tunnel]            : tunnel mode
  -X [--listen-once]       : listen-once mode (useful for debugging)
  -r [--root] ARG          : root of directory to serve
  -R [--read-only]         : force read only, overriding repository config file
  --config-file ARG        : read configuration from file ARG
  --listen-port ARG        : listen port. The default port is 3690.
                             [mode: daemon, listen-once]
  --listen-host ARG        : listen hostname or IP address
                             By default svnserve listens on all addresses.
                             [mode: daemon, listen-once]
  -6 [--prefer-ipv6]       : prefer IPv6 when resolving the listen hostname
                             [IPv4 is preferred by default. Using IPv4 and IPv6
                             at the same time is not supported in daemon mode.
                             Use inetd mode or tunnel mode if you need this.]
  -c [--compression] ARG   : compression level to use for network transmissions
                             [0 .. no compression, 5 .. default, 
                              9 .. maximum compression]
  -M [--memory-cache-size] ARG : size of the extra in-memory cache in MB used to
                             minimize redundant operations.
                             Default is 16.
                             0 switches to dynamically sized caches.
                             [used for FSFS and FSX repositories only]
  --cache-txdeltas ARG     : enable or disable caching of deltas between older
                             revisions.
                             Default is yes.
                             [used for FSFS and FSX repositories only]
  --cache-fulltexts ARG    : enable or disable caching of file contents
                             Default is yes.
                             [used for FSFS and FSX repositories only]
  --cache-revprops ARG     : enable or disable caching of revision properties.
                             Consult the documentation before activating this.
                             Default is no.
                             [used for FSFS and FSX repositories only]
  --client-speed ARG       : Optimize network handling based on the assumption
                             that most clients are connected with a bitrate of
                             ARG Mbit/s.
                             Default is 0 (optimizations disabled).
  --block-read ARG         : Parse and cache all data found in block instead
                             of just the requested item.
                             Default is no.
                             [used for FSFS repositories in 1.9 format only]
  -T [--threads]           : use threads instead of fork [mode: daemon]
  --min-threads ARG        : Minimum number of server threads, even if idle.
                             Capped to max-threads; minimum value is 0.
                             Default is 1.
                             [used only with --threads]
  --max-threads ARG        : Maximum number of server threads, even if there
                             are more connections.  Minimum value is 1.
                             Default is 256.
                             [used only with --threads]
  --foreground             : run in foreground (useful for debugging)
                             [mode: daemon]
  --single-thread          : handle one connection at a time in the parent
                             process (useful for debugging)
  --log-file ARG           : svnserve log file
  --pid-file ARG           : write server process ID to file ARG
                             [mode: daemon, listen-once]
  --tunnel-user ARG        : tunnel username (default is current uid's name)
                             [mode: tunnel]
  -h [--help]              : display this help
  --virtual-host           : virtual host mode (look for repo in directory
                             of provided hostname)
  --version                : show program version information
  -q [--quiet]             : no progress (only errors) to stderr


~~~
