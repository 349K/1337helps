# dpkg-gensymbols command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-gensymbols [<option>...]

Options:
  -p<package>              generate symbols file for package.
  -P<package-build-dir>    temporary build directory instead of debian/tmp.
  -e<library>              explicitly list libraries to scan.
  -v<version>              version of the packages (defaults to
                           version extracted from debian/changelog).
  -c<level>                compare generated symbols file with the reference
                           template in the debian directory and fail if
                           difference is too important; level goes from 0 for
                           no check, to 4 for all checks (default level is 1).
  -q                       keep quiet and never emit any warnings or
                           generate a diff between generated symbols
                           file and the reference template.
  -I<file>                 force usage of <file> as reference symbols
                           file instead of the default file.
  -O[<file>]               write to stdout (or <file>), not .../DEBIAN/symbols.
  -t                       write in template mode (tags are not
                           processed and included in output).
  -V                       verbose output; write deprecated symbols and pattern
                           matching symbols as comments (in template mode only).
  -a<arch>                 assume <arch> as host architecture when processing
                           symbol files.
  -d                       display debug information during work.
  -?, --help               show this help message.
      --version            show the version.

~~~
