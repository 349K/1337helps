# ntpdc command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

ntpdc - vendor-specific NTPD control program - Ver. 4.2.8p8
Usage:  ntpdc [ -<flag> [<val>] | --<name>[{=| }<val>] ]... [ host ...]
  Flg Arg Option-Name    Description
   -4 no  ipv4           Force IPv4 DNS name resolution
				- prohibits the option 'ipv6'
   -6 no  ipv6           Force IPv6 DNS name resolution
				- prohibits the option 'ipv4'
   -c Str command        run a command and exit
				- may appear multiple times
   -d no  debug-level    Increase debug verbosity level
				- may appear multiple times
   -D Num set-debug-level Set the debug verbosity level
				- may appear multiple times
   -i no  interactive    Force ntpq to operate in interactive mode
				- prohibits these options:
				command
				listpeers
				peers
				showpeers
   -l no  listpeers      Print a list of the peers
				- prohibits the option 'command'
   -n no  numeric        numeric host addresses
   -p no  peers          Print a list of the peers
				- prohibits the option 'command'
   -s no  showpeers      Show a list of the peers
				- prohibits the option 'command'
      opt version        output version information and exit
   -? no  help           display extended usage information and exit
   -! no  more-help      extended usage information passed thru pager
   -> opt save-opts      save the option state to a config file
   -< Str load-opts      load options from a config file
				- disabled as '--no-load-opts'
				- may appear multiple times

Options are specified by doubled hyphens and their name or by a single
hyphen and the flag character.


The following option preset mechanisms are supported:
 - reading file $HOME/.ntprc
 - reading file ./.ntprc
 - examining environment variables named NTPDC_*

Please send bug reports to:  <http://bugs.ntp.org, bugs@ntp.org>

~~~
