# intel-virtual-output command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: intel-virtual-output [OPTION]... [TARGET_DISPLAY]...
  -d <source display>  source display
  -f                   keep in foreground (do not detach from console and daemonize)
  -b                   start bumblebee
  -a                   connect to all local displays (e.g. :1, :2, etc)
  -S                   disable use of a singleton and launch a fresh intel-virtual-output process
  -v                   all verbose output, implies -f
  -V <category>        specific verbose output, implies -f
  -h                   this help
If no target displays are parsed on the commandline, 
intel-virtual-output will attempt to connect to any local display
and then start bumblebee.

~~~
