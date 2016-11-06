# mysql_convert_table_format command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

/usr/bin/mysql_convert_table_format  version 1.1

Conversion of a MySQL tables to other storage engines

 Usage: /usr/bin/mysql_convert_table_format database [table[ table ...]]
 If no tables has been specifed, all tables in the database will be converted.
 You can also use wildcards, ie "my%"

 The following options are available:

-f, --force
  Continue even if there is some error.

-?, --help
  Shows this help

-e, --engine=ENGINE
  Converts tables to the given storage engine (Default: MYISAM)

-h, --host=HOST
  Host name where the database server is located. (Default: localhost)

-p, --password=PASSWORD
  Password for the current user.

-P, --port=PORT
  TCP/IP port to connect to if host is not "localhost".

-S, --socket=SOCKET
  Socket to connect with.

-u, --user=USER
  User name to log into the SQL server.

-v, --verbose
  This is a test specific option that is only used when debugging a test.
  Print more information about what is going on.

-V, --version
  Shows the version of this program.

~~~
