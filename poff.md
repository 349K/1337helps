# poff command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


usage: /usr/bin/poff [option] [provider]
options:
  -r        Cause pppd to drop the line and redial.
  -d        Toggle the state of pppd's debug option.
  -c        Cause pppd to renegotiate compression.
  -a        Stop all pppd's.  'provider' will be ignored.
  -h        Print this help summary and exit.
  -v        Print version and exit.
  none      Stop pppd.

Options may not be combined.

If 'provider' is omitted pppd will be stopped or signalled if and only if
there is exactly one running unless the '-a' option was given.  If
'provider' is supplied the pppd controlling the connection to that
provider will be stopped or signalled.

~~~
