# mysql_find_rows command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


/usr/bin/mysql_find_rows  Ver 1.02

Prints all SQL queries that matches a regexp or contains a 'use
database' or 'set ..' command to stdout.  A SQL query may contain
newlines.  This is useful to find things in a MySQL update log.

/usr/bin/mysql_find_rows takes the following options:

--help or --Information
  Shows this help

--regexp=#
  Print queries that matches this.

--start_row=#
  Start output from this row (first row = 1)

--skip-use-db
  Don't include 'use database' commands in the output.

--rows=#
  Quit after this many rows.

Example:

/usr/bin/mysql_find_rows --regexp "problem_table" < update.log

/usr/bin/mysql_find_rows --regexp "problem_table" update-log.1 update-log.2

~~~
