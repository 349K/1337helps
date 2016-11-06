# dpkg-query command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-query [<option> ...] <command>

Commands:
  -s|--status <package> ...        Display package status details.
  -p|--print-avail <package> ...   Display available version details.
  -L|--listfiles <package> ...     List files 'owned' by package(s).
  -l|--list [<pattern> ...]        List packages concisely.
  -W|--show [<pattern> ...]        Show information on package(s).
  -S|--search <pattern> ...        Find package(s) owning file(s).
     --control-list <package>      Print the package control file list.
     --control-show <package> <file>
                                   Show the package control file.
  -c|--control-path <package> [<file>]
                                   Print path for package control file.

  -?, --help                       Show this help message.
      --version                    Show the version.

Options:
  --admindir=<directory>           Use <directory> instead of /var/lib/dpkg.
  --load-avail                     Use available file on --show and --list.
  -f|--showformat=<format>         Use alternative format for --show.

Format syntax:
  A format is a string that will be output for each package. The format
  can include the standard escape sequences \n (newline), \r (carriage
  return) or \\ (plain backslash). Package information can be included
  by inserting variable references to package fields using the ${var[;width]}
  syntax. Fields will be right-aligned unless the width is negative in which
  case left alignment will be used.

~~~
