# runcon command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: runcon CONTEXT COMMAND [args]
  or:  runcon [ -c ] [-u USER] [-r ROLE] [-t TYPE] [-l RANGE] COMMAND [args]
Run a program in a different SELinux security context.
With neither CONTEXT nor COMMAND, print the current security context.

Mandatory arguments to long options are mandatory for short options too.
  CONTEXT            Complete security context
  -c, --compute      compute process transition context before modifying
  -t, --type=TYPE    type (for same role as parent)
  -u, --user=USER    user identity
  -r, --role=ROLE    role
  -l, --range=RANGE  levelrange

      --help     display this help and exit
      --version  output version information and exit

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Full documentation at: <http://www.gnu.org/software/coreutils/runcon>
or available locally via: info '(coreutils) runcon invocation'

~~~
