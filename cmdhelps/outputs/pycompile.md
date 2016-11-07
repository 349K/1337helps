# pycompile command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: pycompile [-V [X.Y][-][A.B]] DIR_OR_FILE [-X REGEXPR]
       pycompile -p PACKAGE

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -v, --verbose         turn verbose mode on
  -q, --quiet           be quiet
  -f, --force           force rebuild even if timestamps are up-to-date
  -O                    byte-compile to .pyo files
  -p PACKAGE, --package=PACKAGE
                        specify Debian package name whose files should be
                        bytecompiled
  -V VRANGE             force private modules to be bytecompiled with Python
                        version from given range, regardless of the default
                        Python version in the system. If there are no other
                        options, bytecompile all public modules for installed
                        Python versions that match given range.  VERSION_RANGE
                        examples: '2.5' (version 2.5 only), '2.5-' (version
                        2.5 or newer), '2.5-2.7' (version 2.5 or 2.6), '-3.0'
                        (all supported 2.X versions)
  -X REGEXPR, --exclude=REGEXPR
                        exclude items that match given REGEXPR. You may use
                        this option multiple times to build up a list of
                        things to exclude.

~~~
