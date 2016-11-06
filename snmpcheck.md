# snmpcheck command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~



Usage:  snmpcheck [-x] [-n|y] [-h] [-H] [-V NUM] [-L] [-f] [[-a] HOSTS] 

  -h	Display this message.
  -a	check error log file AND hosts specified on command line.
  -p	Don't try and ping-echo the host first
  -f	Only check for things I can fix
  HOSTS	check these hosts for problems.

X Options:
  -x	forces ascii base if $DISPLAY set (instead of tk).
  -H	start in hidden mode.  (hides user interface)
  -V NUM	sets the initial verbosity level of the command log (def: 1)
  -L	Show the log window at startup
  -d	Don't start by checking anything.  Just bring up the interface.

Ascii Options:
  -n	Don't ever try and fix the problems found.  Just list.
  -y	Always fix problems found.


~~~
