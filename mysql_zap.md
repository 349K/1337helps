# mysql_zap command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:   /usr/bin/mysql_zap [-signal] [-?Ift] [--help] pattern
Options: -I or -? "info"  -f "force" -t "test".

Version 1.0
Kill processes that match the pattern.
If -f isn't given, ask user for confirmation for each process to kill.
If signal isn't given, try first with signal 15, then with signal 9.
If -t is given, the processes are only shown on stdout.

~~~
