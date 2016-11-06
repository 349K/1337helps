# systemd-analyze command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


systemd-analyze [OPTIONS...] {COMMAND} ...

Profile systemd, show unit dependencies, check unit files.

  -h --help               Show this help
     --version            Show package version
     --no-pager           Do not pipe output into a pager
     --system             Operate on system systemd instance
     --user               Operate on user systemd instance
  -H --host=[USER@]HOST   Operate on remote host
  -M --machine=CONTAINER  Operate on local container
     --order              Show only order in the graph
     --require            Show only requirement in the graph
     --from-pattern=GLOB  Show only origins in the graph
     --to-pattern=GLOB    Show only destinations in the graph
     --fuzz=SECONDS       Also print also services which finished SECONDS
                          earlier than the latest in the branch
     --man[=BOOL]         Do [not] check for existence of man pages

Commands:
  time                    Print time spent in the kernel
  blame                   Print list of running units ordered by time to init
  critical-chain          Print a tree of the time critical chain of units
  plot                    Output SVG graphic showing service initialization
  dot                     Output dependency graph in dot(1) format
  set-log-level LEVEL     Set logging threshold for manager
  set-log-target TARGET   Set logging target for manager
  dump                    Output state serialization of service manager
  verify FILE...          Check unit files for correctness

~~~
