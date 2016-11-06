# mysqlreport command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


mysqlreport v3.5 Apr 16 2008
mysqlreport makes an easy-to-read report of important MySQL status values.

Command line options (abbreviations work):
   --user USER       Connect to MySQL as USER
   --password PASS   Use PASS or prompt for MySQL user's password
   --host ADDRESS    Connect to MySQL at ADDRESS
   --port PORT       Connect to MySQL at PORT
   --socket SOCKET   Connect to MySQL at SOCKET
   --no-mycnf        Don't read ~/.my.cnf
   --infile FILE     Read status values from FILE instead of MySQL
   --outfile FILE    Write report to FILE
   --email ADDRESS   Email report to ADDRESS (doesn't work on Windows)
   --flush-status    Issue FLUSH STATUS; after getting current values
   --relative X      Generate relative reports. If X is an integer,
                     reports are live from the MySQL server X seconds apart.
                     If X is a list of infiles (file1 file2 etc.),
                     reports are generated from the infiles in the order
                     that they are given.
   --report-count N  Collect N number of live relative reports (default 1)
   --detach          Fork and detach from terminal (run in background)
   --help            Prints this
   --debug           Print debugging information

Visit http://hackmysql.com/mysqlreport for more information.

~~~
