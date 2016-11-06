# reindexdb command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

reindexdb reindexes a PostgreSQL database.

Usage:
  reindexdb [OPTION]... [DBNAME]

Options:
  -a, --all                 reindex all databases
  -d, --dbname=DBNAME       database to reindex
  -e, --echo                show the commands being sent to the server
  -i, --index=INDEX         recreate specific index(es) only
  -q, --quiet               don't write any messages
  -s, --system              reindex system catalogs
  -S, --schema=SCHEMA       reindex specific schema(s) only
  -t, --table=TABLE         reindex specific table(s) only
  -v, --verbose             write a lot of output
  -V, --version             output version information, then exit
  -?, --help                show this help, then exit

Connection options:
  -h, --host=HOSTNAME       database server host or socket directory
  -p, --port=PORT           database server port
  -U, --username=USERNAME   user name to connect as
  -w, --no-password         never prompt for password
  -W, --password            force password prompt
  --maintenance-db=DBNAME   alternate maintenance database

Read the description of the SQL command REINDEX for details.

Report bugs to <pgsql-bugs@postgresql.org>.

~~~
