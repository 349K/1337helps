# pon command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: pon [OPTIONS] [provider] [arguments]
  -q|--quick           pppd hangs up after all ip-up scripts are run

If pon is invoked without arguments, /etc/ppp/ppp_on_boot file will be
run, presuming it exists and is executable. Otherwise, a PPP connection
will be started using settings from /etc/ppp/peers/provider.
If you specify one argument, a PPP connection will be started using
settings from the appropriate file in the /etc/ppp/peers/ directory, and
any additional arguments supplied will be passed as extra arguments to
pppd.


~~~
