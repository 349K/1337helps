# pg_receivexlog command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

pg_receivexlog receives PostgreSQL streaming transaction logs.

Usage:
  pg_receivexlog [OPTION]...

Options:
  -D, --directory=DIR    receive transaction log files into this directory
      --if-not-exists    do not error if slot already exists when creating a slot
  -n, --no-loop          do not loop on connection lost
  -s, --status-interval=SECS
                         time between status packets sent to server (default: 10)
  -S, --slot=SLOTNAME    replication slot to use
      --synchronous      flush transaction log immediately after writing
  -v, --verbose          output verbose messages
  -V, --version          output version information, then exit
  -?, --help             show this help, then exit

Connection options:
  -d, --dbname=CONNSTR   connection string
  -h, --host=HOSTNAME    database server host or socket directory
  -p, --port=PORT        database server port number
  -U, --username=NAME    connect as specified database user
  -w, --no-password      never prompt for password
  -W, --password         force password prompt (should happen automatically)

Optional actions:
      --create-slot      create a new replication slot (for the slot's name see --slot)
      --drop-slot        drop the replication slot (for the slot's name see --slot)

Report bugs to <pgsql-bugs@postgresql.org>.

~~~
