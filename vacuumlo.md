# vacuumlo command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

vacuumlo removes unreferenced large objects from databases.

Usage:
  vacuumlo [OPTION]... DBNAME...

Options:
  -l LIMIT       commit after removing each LIMIT large objects
  -n             don't remove large objects, just show what would be done
  -v             write a lot of progress messages
  -V, --version  output version information, then exit
  -?, --help     show this help, then exit

Connection options:
  -h HOSTNAME    database server host or socket directory
  -p PORT        database server port
  -U USERNAME    user name to connect as
  -w             never prompt for password
  -W             force password prompt

Report bugs to <pgsql-bugs@postgresql.org>.

~~~
