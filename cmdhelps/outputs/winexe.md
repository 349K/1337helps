# winexe command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: winexe [OPTION]... //HOST COMMAND
Options:
  -h, --help                                  Display help message
  -V, --version                               Display version number
  -U, --user=[DOMAIN/]USERNAME[%PASSWORD]     Set the network username
  -A, --authentication-file=FILE              Get the credentials from a file
  -N, --no-pass                               Do not ask for a password
  -k, --kerberos=STRING                       Use Kerberos, -k [yes|no]
  -d, --debuglevel=DEBUGLEVEL                 Set debug level
      --uninstall                             Uninstall winexe service after
                                              remote execution
      --reinstall                             Reinstall winexe service before
                                              remote execution
      --system                                Use SYSTEM account
      --profile                               Load user profile
      --convert                               Try to convert characters
                                              between local and remote
                                              code-pages
      --runas=[DOMAIN\]USERNAME%PASSWORD      Run as the given user (BEWARE:
                                              this password is sent in
                                              cleartext over the network!)
      --runas-file=FILE                       Run as user options defined in a
                                              file
      --interactive=0|1                       Desktop interaction: 0 -
                                              disallow, 1 - allow. If allow,
                                              also use the --system switch
                                              (Windows requirement). Vista
                                              does not support this option.
      --ostype=0|1|2                          OS type: 0 - 32-bit, 1 - 64-bit,
                                              2 - winexe will decide.
                                              Determines which version (32-bit
                                              or 64-bit) of service will be
                                              installed.

~~~
