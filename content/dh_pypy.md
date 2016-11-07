# dh_pypy command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dh_pypy -p PACKAGE [-V [X.Y][-][A.B]] DIR [-X REGEXPR]


Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  --no-guessing-deps    disable guessing dependencies
  --skip-private        don't check private directories
  -v, --verbose         turn verbose mode on
  -i, --indep           act on architecture independent packages
  -a, -s, --arch        act on architecture dependent packages
  -q, --quiet           be quiet
  -p PACKAGE, --package=PACKAGE
                        act on the package named PACKAGE
  -N NO_PACKAGE, --no-package=NO_PACKAGE
                        do not act on the specified package
  --compile-all         compile all files from given private directory in
                        postinst, not just the ones provided by the package
  -X REGEXPR, --exclude=REGEXPR
                        exclude items that match given REGEXPR. You may use
                        this option multiple times to build up a list of
                        things to exclude.
  --depends=DEPENDS     translate given requirements into Debian dependencies
                        and add them to ${pypy:Depends}. Use it for missing
                        items in requires.txt.
  --depends-section=DEPENDS_SECTION
                        translate requirements from given section into Debian
                        dependencies and add them to ${python3:Depends}
  --recommends=RECOMMENDS
                        translate given requirements into Debian dependencies
                        and add them to ${pypy:Recommends}
  --recommends-section=RECOMMENDS_SECTION
                        translate requirements from given section into Debian
                        dependencies and add them to ${python3:Recommends}
  --suggests=SUGGESTS   translate given requirements into Debian dependencies
                        and add them to ${pypy:Suggests}
  --suggests-section=SUGGESTS_SECTION
                        translate requirements from given section into Debian
                        dependencies and add them to ${python3:Suggests}
  --requires=REQUIRES   translate requirements from given file into Debian
                        dependencies and add them to ${pypy:Depends}
  --shebang=SHEBANG     use given command as shebang in scripts
  --ignore-shebangs     do not translate shebangs into Debian dependencies
  --no-dbg-cleaning     do not remove files from debug packages
  --no-ext-rename       do not add magic tags nor multiarch tuples to
                        extension file names)
  --no-shebang-rewrite  do not rewrite shebangs

~~~
