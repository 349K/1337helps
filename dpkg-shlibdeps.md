# dpkg-shlibdeps command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-shlibdeps [<option>...] <executable>|-e<executable> [<option>...]

Positional options (order is significant):
  <executable>             include dependencies for <executable>,
  -e<executable>           (use -e if <executable> starts with '-')
  -d<dependency-field>     next executable(s) set shlibs:<dependency-field>.

Options:
  -l<library-dir>          add directory to private shared library search list.
  -p<varname-prefix>       set <varname-prefix>:* instead of shlibs:*.
  -O[<file>]               write variable settings to stdout (or <file>).
  -L<local-shlibs-file>    shlibs override file, not debian/shlibs.local.
  -T<substvars-file>       update variables here, not debian/substvars.
  -t<type>                 set package type (default is deb).
  -x<package>              exclude package from the generated dependencies.
  -S<package-build-dir>    search needed libraries in the given
                             package build directory first.
  -I<package-build-dir>    ignore needed libraries, shlibs and symbols files
                             in the given build directory.
  -v                       enable verbose mode (can be used multiple times).
  --ignore-missing-info    don't fail if dependency information can't be found.
  --warnings=<value>       define set of active warnings (see manual page).
  --admindir=<directory>   change the administrative directory.
  -?, --help               show this help message.
      --version            show the version.

Dependency fields recognized are:
  Suggests/Recommends/Depends/Pre-Depends

~~~
