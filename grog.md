# grog command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: grog [option]... [--] [filespec]...

"filespec" is either the name of an existing, readable file or "-" for
standard input.  If no `filespec' is specified, standard input is
assumed automatically.  All arguments after a `--' are regarded as file
names, even if they start with a `-' character.

`option' is either a `groff' option or one of these:

-h|--help	print this uasge message and exit
-v|--version	print version information and exit

-C		compatibility mode
--ligatures	include options `-P-y -PU' for internal font, which
		preserverses the ligatures like `fi'
--run		run the checked-out groff command
--warnings	display more warnings to standard error

All other options should be `groff' 1-character options.  These are then
appended to the generated `groff' command line.  The `-m' options will
be checked by `grog'.



~~~
