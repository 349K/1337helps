# x86_64-linux-gnu-c++filt command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: x86_64-linux-gnu-c++filt [options] [mangled names]
Options are:
  [-_|--strip-underscore]     Ignore first leading underscore
  [-n|--no-strip-underscore]  Do not ignore a leading underscore (default)
  [-p|--no-params]            Do not display function arguments
  [-i|--no-verbose]           Do not show implementation details (if any)
  [-t|--types]                Also attempt to demangle type encodings
  [-s|--format {none,auto,gnu,lucid,arm,hp,edg,gnu-v3,java,gnat,dlang}]
  [@<file>]                   Read extra options from <file>
  [-h|--help]                 Display this information
  [-v|--version]              Show the version information
Demangled names are displayed to stdout.
If a name cannot be demangled it is just echoed to stdout.
If no names are provided on the command line, stdin is read.
Report bugs to <http://www.sourceware.org/bugzilla/>.

~~~
