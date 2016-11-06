# myisampack command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

myisampack Ver 1.23 for debian-linux-gnu on x86_64
Copyright 2002-2008 MySQL AB, 2008 Sun Microsystems, Inc.
This software comes with ABSOLUTELY NO WARRANTY. This is free software,
and you are welcome to modify and redistribute it under the GPL license

Pack a MyISAM-table to take much less space.
Keys are not updated, you must run myisamchk -rq on the datafile
afterwards to update the keys.
You should give the .MYI file as the filename argument.

Usage: myisampack [OPTIONS] filename...
  -b, --backup        Make a backup of the table as table_name.OLD.
  --character-sets-dir=name 
                      Directory where character sets are.
  -#, --debug[=name]  Output debug log. Often this is 'd:t:o,filename'.
  -f, --force         Force packing of table even if it gets bigger or if
                      tempfile exists.
  -j, --join=name     Join all given tables into 'new_table_name'. All tables
                      MUST have identical layouts.
  -?, --help          Display this help and exit.
  -s, --silent        Be more silent.
  -T, --tmpdir=name   Use temporary directory to store temporary table.
  -t, --test          Don't pack table, only test packing it.
  -v, --verbose       Write info about progress and packing result. Use many -v
                      for more verbosity!
  -V, --version       Output version information and exit.
  -w, --wait          Wait and retry if table is in use.

Default options are read from the following files in the given order:
/etc/my.cnf /etc/mysql/my.cnf /usr/etc/my.cnf ~/.my.cnf 
The following groups are read: myisampack
The following options may be given as the first argument:
--print-defaults        Print the program argument list and exit.
--no-defaults           Don't read default options from any option file,
                        except for login file.
--defaults-file=#       Only read default options from the given file #.
--defaults-extra-file=# Read this file after the global files are read.
--defaults-group-suffix=#
                        Also read groups with concat(group, suffix)
--login-path=#          Read this path from the login file.

Variables (--variable-name=value)
and boolean options {FALSE|TRUE}  Value (after reading options)
--------------------------------- ----------------------------------------
backup                            FALSE
character-sets-dir                (No default value)
join                              (No default value)
wait                              FALSE

~~~
