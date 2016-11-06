# sqldiff command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: sqldiff [options] DB1 DB2
Output SQL text that would transform DB1 into DB2.
Options:
  --changeset FILE      Write a CHANGESET into FILE
  -L|--lib LIBRARY      Load an SQLite extension library
  --primarykey          Use schema-defined PRIMARY KEYs
  --rbu                 Output SQL to create/populate RBU table(s)
  --schema              Show only differences in the schema
  --summary             Show only a summary of the differences
  --table TAB           Show only differences in table TAB
  --transaction         Show SQL output inside a transaction
  --vtab                Handle fts3, fts4, fts5 and rtree tables

~~~
