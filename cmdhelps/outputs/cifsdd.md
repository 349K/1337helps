# cifsdd command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: cifsdd [OPTION...]

Help options:
  -?, --help                                  Show this help message
      --usage                                 Display brief usage message

Common Samba options:
  -d, --debuglevel=DEBUGLEVEL                 Set debug level
      --debug-stderr                          Send debug output to STDERR
  -s, --configfile=CONFIGFILE                 Use alternative configuration
                                              file
      --option=name=value                     Set smb.conf option from command
                                              line
  -l, --log-basename=LOGFILEBASE              Basename for log/debug files
      --leak-report                           enable talloc leak reporting on
                                              exit
      --leak-report-full                      enable full talloc leak
                                              reporting on exit

Connection options:
  -R, --name-resolve=NAME-RESOLVE-ORDER       Use these name resolution
                                              services only
  -O, --socket-options=SOCKETOPTIONS          socket options to use
  -n, --netbiosname=NETBIOSNAME               Primary netbios name
  -S, --signing=on|off|required               Set the client signing state
  -W, --workgroup=WORKGROUP                   Set the workgroup name
      --realm=REALM                           Set the realm name
  -i, --scope=SCOPE                           Use this Netbios scope
  -m, --maxprotocol=MAXPROTOCOL               Set max protocol level

Authentication options:
  -U, --user=[DOMAIN/]USERNAME[%PASSWORD]     Set the network username
  -N, --no-pass                               Don't ask for a password
      --password=STRING                       Password
  -A, --authentication-file=FILE              Get the credentials from a file
  -P, --machine-pass                          Use stored machine account
                                              password
      --simple-bind-dn=STRING                 DN to use for a simple bind
  -k, --kerberos=STRING                       Use Kerberos, -k [yes|no]
      --krb5-ccache=STRING                    Credentials cache location for
                                              Kerberos
  -S, --sign                                  Sign connection to prevent
                                              modification in transit
  -e, --encrypt                               Encrypt connection for privacy

Version options:
  -V, --version                               Print version

CIFS dd options:
  bs=SIZE                force ibs and obs to SIZE bytes
  ibs=SIZE               read SIZE bytes at a time
  obs=SIZE               write SIZE bytes at a time
  count=COUNT            copy COUNT input blocks
  seek=COUNT             skip COUNT blocks at start of output
  skip=COUNT             skip COUNT blocks at start of input
  if=FILE                read input from FILE
  of=FILE                write output to FILE
  direct=BOOLEAN         use direct I/O if non-zero
  sync=BOOLEAN           use synchronous writes if non-zero
  oplock=BOOLEAN         take oplocks on the input and output files

FILE can be a local filename or a UNC path of the form //server/share/path.


~~~
