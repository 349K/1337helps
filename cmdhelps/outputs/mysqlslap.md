# mysqlslap command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

mysqlslap  Ver 1.0 Distrib 5.6.30, for debian-linux-gnu (x86_64)
Copyright (c) 2005, 2016, Oracle and/or its affiliates. All rights reserved.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Run a query multiple times against the server.

Usage: mysqlslap [OPTIONS]

Default options are read from the following files in the given order:
/etc/my.cnf /etc/mysql/my.cnf /usr/etc/my.cnf ~/.my.cnf 
The following groups are read: mysqlslap client
The following options may be given as the first argument:
--print-defaults        Print the program argument list and exit.
--no-defaults           Don't read default options from any option file,
                        except for login file.
--defaults-file=#       Only read default options from the given file #.
--defaults-extra-file=# Read this file after the global files are read.
--defaults-group-suffix=#
                        Also read groups with concat(group, suffix)
--login-path=#          Read this path from the login file.
  -?, --help          Display this help and exit.
  -a, --auto-generate-sql 
                      Generate SQL where not supplied by file or command line.
  --auto-generate-sql-add-autoincrement 
                      Add an AUTO_INCREMENT column to auto-generated tables.
  --auto-generate-sql-execute-number=# 
                      Set this number to generate a set number of queries to
                      run.
  --auto-generate-sql-guid-primary 
                      Add GUID based primary keys to auto-generated tables.
  --auto-generate-sql-load-type=name 
                      Specify test load type: mixed, update, write, key, or
                      read; default is mixed.
  --auto-generate-sql-secondary-indexes=# 
                      Number of secondary indexes to add to auto-generated
                      tables.
  --auto-generate-sql-unique-query-number=# 
                      Number of unique queries to generate for automatic tests.
  --auto-generate-sql-unique-write-number=# 
                      Number of unique queries to generate for
                      auto-generate-sql-write-number.
  --auto-generate-sql-write-number=# 
                      Number of row inserts to perform for each thread (default
                      is 100).
  --commit=#          Commit records every X number of statements.
  -C, --compress      Use compression in server/client protocol.
  -c, --concurrency=name 
                      Number of clients to simulate for query to run.
  --create=name       File or string to use create tables.
  --create-schema=name 
                      Schema to run tests in.
  --csv[=name]        Generate CSV output to named file or to stdout if no file
                      is named.
  -#, --debug[=#]     This is a non-debug version. Catch this and exit.
  --debug-check       Check memory and open file usage at exit.
  -T, --debug-info    Print some debug info at exit.
  --default-auth=name Default authentication client-side plugin to use.
  -F, --delimiter=name 
                      Delimiter to use in SQL statements supplied in file or
                      command line.
  --detach=#          Detach (close and reopen) connections after X number of
                      requests.
  --enable-cleartext-plugin 
                      Enable/disable the clear text authentication plugin.
  -e, --engine=name   Storage engine to use for creating the table.
  -h, --host=name     Connect to host.
  -i, --iterations=#  Number of times to run the tests.
  --no-drop           Do not drop the schema after the test.
  -x, --number-char-cols=name 
                      Number of VARCHAR columns to create in table if
                      specifying --auto-generate-sql.
  -y, --number-int-cols=name 
                      Number of INT columns to create in table if specifying
                      --auto-generate-sql.
  --number-of-queries=# 
                      Limit each client to this number of queries (this is not
                      exact).
  --only-print        Do not connect to the databases, but instead print out
                      what would have been done.
  -p, --password[=name] 
                      Password to use when connecting to server. If password is
                      not given it's asked from the tty.
  --plugin-dir=name   Directory for client-side plugins.
  -P, --port=#        Port number to use for connection.
  --post-query=name   Query to run or file containing query to execute after
                      tests have completed.
  --post-system=name  system() string to execute after tests have completed.
  --pre-query=name    Query to run or file containing query to execute before
                      running tests.
  --pre-system=name   system() string to execute before running tests.
  --protocol=name     The protocol to use for connection (tcp, socket, pipe,
                      memory).
  -q, --query=name    Query to run or file containing query to run.
  --secure-auth       Refuse client connecting to server if it uses old
                      (pre-4.1.1) protocol.
                      (Defaults to on; use --skip-secure-auth to disable.)
  -s, --silent        Run program in silent mode - no output.
  -S, --socket=name   The socket file to use for connection.
  --ssl               Enable SSL for connection (automatically enabled with
                      other flags).
  --ssl-ca=name       CA file in PEM format (check OpenSSL docs, implies
                      --ssl).
  --ssl-capath=name   CA directory (check OpenSSL docs, implies --ssl).
  --ssl-cert=name     X509 cert in PEM format (implies --ssl).
  --ssl-cipher=name   SSL cipher to use (implies --ssl).
  --ssl-key=name      X509 key in PEM format (implies --ssl).
  --ssl-crl=name      Certificate revocation list (implies --ssl).
  --ssl-crlpath=name  Certificate revocation list path (implies --ssl).
  --ssl-verify-server-cert 
                      Verify server's "Common Name" in its cert against
                      hostname used when connecting. This option is disabled by
                      default.
  --ssl-mode=name     SSL connection mode.
  -u, --user=name     User for login if not current user.
  -v, --verbose       More verbose output; you can use this multiple times to
                      get even more verbose output.
  -V, --version       Output version information and exit.

~~~
