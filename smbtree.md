# smbtree command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: [OPTION...]
  -b, --broadcast                    Use broadcast instead of using the master
                                     browser
  -D, --domains                      List only domains (workgroups) of tree
  -S, --servers                      List domains(workgroups) and servers of
                                     tree

Help options:
  -?, --help                         Show this help message
      --usage                        Display brief usage message

Common samba options:
  -d, --debuglevel=DEBUGLEVEL        Set debug level
  -s, --configfile=CONFIGFILE        Use alternate configuration file
  -l, --log-basename=LOGFILEBASE     Base name for log files
  -V, --version                      Print version
      --option=name=value            Set smb.conf option from command line

Authentication options:
  -U, --user=USERNAME                Set the network username
  -N, --no-pass                      Don't ask for a password
  -k, --kerberos                     Use kerberos (active directory)
                                     authentication
  -A, --authentication-file=FILE     Get the credentials from a file
  -S, --signing=on|off|required      Set the client signing state
  -P, --machine-pass                 Use stored machine account password
  -e, --encrypt                      Encrypt SMB transport
  -C, --use-ccache                   Use the winbind ccache for authentication
      --pw-nt-hash                   The supplied password is the NT hash

~~~
