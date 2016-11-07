# dropuser command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

dropuser removes a PostgreSQL role.

Usage:
  dropuser [OPTION]... [ROLENAME]

Options:
  -e, --echo                show the commands being sent to the server
  -i, --interactive         prompt before deleting anything, and prompt for
                            role name if not specified
  -V, --version             output version information, then exit
  --if-exists               don't report error if user doesn't exist
  -?, --help                show this help, then exit

Connection options:
  -h, --host=HOSTNAME       database server host or socket directory
  -p, --port=PORT           database server port
  -U, --username=USERNAME   user name to connect as (not the one to drop)
  -w, --no-password         never prompt for password
  -W, --password            force password prompt

Report bugs to <pgsql-bugs@postgresql.org>.

~~~
