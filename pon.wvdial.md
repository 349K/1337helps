# pon.wvdial command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: wvdial [OPTION...] [SECTION]... [OPTION=value]...
An intelligent PPP dialer.

  -c, --chat                 used when running wvdial from pppd
  -C, --config=configfile    use configfile instead of /etc/wvdial.conf
  -n, --no-syslog            don't send output to SYSLOG
  -?, --help                 Give this help list
      --usage                Give a short usage message
  -V, --version              Print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

Optional SECTION arguments refer to sections in configuration file (usually)
/etc/wvdial.conf, $HOME/.wvdialrc or the file specified by --config.
Specified sections are all read, with later ones overriding previous ones.
Any options not in the listed sections are taken from [Dialer Defaults].

Also, optional OPTION=value parameters allow you to override options within
the configuration files.

~~~
