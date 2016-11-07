# clang-rename-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

OVERVIEW: A tool to rename symbols in C/C++ code.
clang-rename renames every occurrence of a symbol found at <offset> in
<source0>. If -i is specified, the edited files are overwritten to disk.
Otherwise, the results are written to stdout.

USAGE: clang-rename-3.6 [options] <source0> [... <sourceN>]

OPTIONS:

Clang-rename options:

  -extra-arg=<string>        - Additional argument to append to the compiler command line
  -extra-arg-before=<string> - Additional argument to prepend to the compiler command line
  -i                         - Overwrite edited <file>s.
  -new-name=<string>         - The new name to change the symbol to.
  -offset=<uint>             - Locates the symbol by offset as opposed to <line>:<column>.
  -p=<string>                - Build path
  -pl                        - Print the locations affected by renaming to stderr.
  -pn                        - Print the found symbol's name prior to renaming to stderr.

General options:

  -help                      - Display available options (-help-hidden for more)
  -help-list                 - Display list of available options (-help-list-hidden for more)
  -version                   - Display the version of this program

~~~
