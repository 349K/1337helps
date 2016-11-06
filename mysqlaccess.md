# mysqlaccess command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

mysqlaccess Version 2.06, 20 Dec 2000
By RUG-AIV, by Yves Carlier (Yves.Carlier@rug.ac.be)
Changes by Steve Harvey (sgh@vex.net)
This software comes with ABSOLUTELY NO WARRANTY.

Warning: mysqlaccess is deprecated and will be removed in a future version.

You have to supply a userid.
You have to supply the name of a database.


Usage: mysqlaccess [host [user [db]]] OPTIONS

  -?, --help           display this helpscreen and exit
  -v, --version        print information on the program `mysqlaccess'

  -u, --user=#         username for logging in to the db
  -p, --password=#     validate password for user
  -h, --host=#         name or IP-number of the host
  -d, --db=#           name of the database

  -U, --superuser=#    connect as superuser
  -P, --spassword=#    password for superuser
  -H, --rhost=#        remote MySQL-server to connect to
      --old_server     connect to old MySQL-server (before v3.21) which 
                       does not yet know how to handle full where clauses.

  -b, --brief          single-line tabular report
  -t, --table          report in table-format

  --relnotes           print release-notes
  --plan               print suggestions/ideas for future releases
  --howto              some examples of how to run `mysqlaccess'
  --debug=N            enter debuglevel N (0..3)

  --copy               reload temporary grant-tables from original ones
  --preview            show differences in privileges after making
                       changes in (temporary) grant-tables
  --commit             copy grant-rules from temporary tables to grant-tables
                       (!don't forget to do an mysqladmin reload)
  --rollback           undo the last changes to the grant-tables.

  Note:
    + At least the user and the db must be given (even with wildcards)
    + If no host is given, `localhost' is assumed
    + Wilcards (*,?,%,_) are allowed for host, user and db, but be sure 
      to escape them from your shell!! (ie type \* or '*')

~~~
