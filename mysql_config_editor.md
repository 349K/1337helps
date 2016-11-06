# mysql_config_editor command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

mysql_config_editor Ver 1.0 Distrib 5.6.30, for debian-linux-gnu on x86_64
Copyright (c) 2012, 2016, Oracle and/or its affiliates. All rights reserved.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

MySQL Configuration Utility.
Usage: mysql_config_editor [program options] [command [command options]]
  -?, --help          Display this help and exit.
  -v, --verbose       Write more information.
  -V, --version       Output version information and exit.

Variables (--variable-name=value)
and boolean options {FALSE|TRUE}  Value (after reading options)
--------------------------------- ----------------------------------------
verbose                           FALSE

Where command can be any one of the following :
       set [command options]     Sets user name/password/host name/socket/port
                                 for a given login path (section).
       remove [command options]  Remove a login path from the login file.
       print [command options]   Print all the options for a specified
                                 login path.
       reset [command options]   Deletes the contents of the login file.
       help                      Display this usage/help information.


~~~
