# sharesec command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: sharesec sharename

  -r, --remove=ACL                   Remove ACEs
  -m, --modify=ACL                   Modify existing ACEs
  -a, --add=ACL                      Add ACEs
  -R, --replace=ACLS                 Overwrite share permission ACL
  -D, --delete                       Delete the entire security descriptor
  -S, --setsddl=STRING               Set the SD in sddl format
  -V, --viewsddl                     View the SD in sddl format
  -v, --view                         View current share permissions
      --view-all                     View all current share permissions
  -M, --machine-sid                  Initialize the machine SID
  -F, --force                        Force storing the ACL

Help options:
  -?, --help                         Show this help message
      --usage                        Display brief usage message

Common samba options:
  -d, --debuglevel=DEBUGLEVEL        Set debug level
  -s, --configfile=CONFIGFILE        Use alternate configuration file
  -l, --log-basename=LOGFILEBASE     Base name for log files
  -V, --version                      Print version
      --option=name=value            Set smb.conf option from command line

~~~
