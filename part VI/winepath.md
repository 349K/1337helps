# winepath command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: winepath [OPTION] [PATH]...
Convert PATH(s) to Unix or Windows long or short paths.

  -u, --unix    converts a Windows path to a Unix path
  -w, --windows converts a Unix path to a long Windows path
  -l, --long    converts the short Windows path of an existing file or
                directory to the long format
  -s, --short   converts the long Windows path of an existing file or
                directory to the short format
  -0            separate output with \0 character, instead of a newline
  -h, --help    output this help message and exit
  -v, --version output version information and exit

If more than one option is given then the input paths are output in
all formats specified, in the order long, short, Unix, Windows.
If no option is given the default is Unix format.

~~~
