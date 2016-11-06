# dpkg-scanpackages command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-scanpackages [<option>...] <binary-path> [<override-file> [<path-prefix>]] > Packages

Options:
  -t, --type <type>        scan for <type> packages (default is 'deb').
  -a, --arch <arch>        architecture to scan for.
  -h, --hash <hash-list>   only generate hashes for the specified list.
  -m, --multiversion       allow multiple versions of a single package.
  -e, --extra-override <file>
                           use extra override file.
  -M, --medium <medium>    add X-Medium field for dselect multicd access method
  -?, --help               show this help message.
      --version            show the version.

~~~
