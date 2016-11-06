# mysql_waitpid command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

mysql_waitpid version 1.1 by Jani Tolonen

usage: mysql_waitpid [options] #pid #time

Description: Waits for a program, which program id is #pid, to
terminate within #time seconds. If the program terminates within
this time, or if the #pid no longer exists, value 0 is returned.
Otherwise 1 is returned. Both #pid and #time must be positive
integer arguments.

Options:
  -?, --help          Display this help and exit.
  -I, --help          Synonym for -?.
  -v, --verbose       Be more verbose. Give a warning, if kill can't handle
                      signal 0.
  -V, --version       Print version information and exit.

~~~
