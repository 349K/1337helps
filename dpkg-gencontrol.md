# dpkg-gencontrol command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-gencontrol [<option>...]

Options:
  -p<package>              print control file for package.
  -c<control-file>         get control info from this file.
  -l<changelog-file>       get per-version info from this file.
  -F<changelog-format>     force changelog format.
  -v<force-version>        set version of binary package.
  -f<files-list-file>      write files here instead of debian/files.
  -P<package-build-dir>    temporary build directory instead of debian/tmp.
  -n<filename>             assume the package filename will be <filename>.
  -O[<file>]               write to stdout (or <file>), not .../DEBIAN/control.
  -is, -ip, -isp, -ips     deprecated, ignored for compatibility.
  -D<field>=<value>        override or add a field and value.
  -U<field>                remove a field.
  -V<name>=<value>         set a substitution variable.
  -T<substvars-file>       read variables here, not debian/substvars.
  -?, --help               show this help message.
      --version            show the version.

~~~
