# envsubst command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: envsubst [OPTION] [SHELL-FORMAT]

Substitutes the values of environment variables.

Operation mode:
  -v, --variables             output the variables occurring in SHELL-FORMAT

Informative output:
  -h, --help                  display this help and exit
  -V, --version               output version information and exit

In normal operation mode, standard input is copied to standard output,
with references to environment variables of the form $VARIABLE or ${VARIABLE}
being replaced with the corresponding values.  If a SHELL-FORMAT is given,
only those environment variables that are referenced in SHELL-FORMAT are
substituted; otherwise all environment variables references occurring in
standard input are substituted.

When --variables is used, standard input is ignored, and the output consists
of the environment variables that are referenced in SHELL-FORMAT, one per line.

Report bugs to <bug-gnu-gettext@gnu.org>.

~~~
