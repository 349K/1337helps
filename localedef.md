# localedef command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: localedef [OPTION...] NAME
  or:  localedef [OPTION...] [--add-to-archive|--delete-from-archive] FILE...
  or:  localedef [OPTION...] --list-archive [FILE]
Compile locale specification

 Input Files:
  -f, --charmap=FILE         Symbolic character names defined in FILE
  -i, --inputfile=FILE       Source definitions are found in FILE
  -u, --repertoire-map=FILE  FILE contains mapping from symbolic names to UCS4
                             values

 Output control:
  -c, --force                Create output even if warning messages were issued
                            
      --posix                Strictly conform to POSIX
      --prefix=PATH          Optional output file prefix
      --quiet                Suppress warnings and information messages
  -v, --verbose              Print more messages

 Archive control:
      --add-to-archive       Add locales named by parameters to archive
  -A, --alias-file=FILE      locale.alias file to consult when making archive
      --big-endian           Generate big-endian output
      --delete-from-archive  Remove locales named by parameters from archive
      --list-archive         List content of archive
      --little-endian        Generate little-endian output
      --no-archive           Don't add new data to archive
      --replace              Replace existing archive content

  -?, --help                 Give this help list
      --usage                Give a short usage message
  -V, --version              Print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

System's directory for character maps : /usr/share/i18n/charmaps
		       repertoire maps: /usr/share/i18n/repertoiremaps
		       locale path    : /usr/lib/locale:/usr/share/i18n
For bug reporting instructions, please see:
<http://www.debian.org/Bugs/>.

~~~
