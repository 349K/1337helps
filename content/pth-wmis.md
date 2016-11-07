# pth-wmis command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: //host

Example: wmis -U [domain/]adminuser%password //host cmd.exe /c dir c:\ > c:\windows\temp\output.txt 

Help options:
  -?, --help                                  Show this help message
  --usage                                     Display brief usage message

Common samba options:
  -d, --debuglevel=DEBUGLEVEL                 Set debug level
  --debug-stderr                              Send debug output to STDERR
  -s, --configfile=CONFIGFILE                 Use alternative configuration
                                              file
  --option=name=value                         Set smb.conf option from command
                                              line
  -l, --log-basename=LOGFILEBASE              Basename for log/debug files
  --leak-report                               enable talloc leak reporting on
                                              exit
  --leak-report-full                          enable full talloc leak
                                              reporting on exit

Connection options:
  -R, --name-resolve=NAME-RESOLVE-ORDER       Use these name resolution
                                              services only
  -O, --socket-options=SOCKETOPTIONS          socket options to use
  -n, --netbiosname=NETBIOSNAME               Primary netbios name
  -W, --workgroup=WORKGROUP                   Set the workgroup name
  --realm=REALM                               Set the realm name
  -i, --scope=SCOPE                           Use this Netbios scope
  -m, --maxprotocol=MAXPROTOCOL               Set max protocol level

Authentication options:
  -U, --user=[DOMAIN\]USERNAME[%PASSWORD]     Set the network username
  -N, --no-pass                               Don't ask for a password
  --password=STRING                           Password
  -A, --authentication-file=FILE              Get the credentials from a file
  -S, --signing=on|off|required               Set the client signing state
  -P, --machine-pass                          Use stored machine account
                                              password (implies -k)
  --simple-bind-dn=STRING                     DN to use for a simple bind
  -k, --kerberos=STRING                       Use Kerberos
  --use-security-mechanisms=STRING            Restricted list of
                                              authentication mechanisms
                                              available for use with this
                                              authentication

Common samba options:
  -V, --version                               Print version

~~~
