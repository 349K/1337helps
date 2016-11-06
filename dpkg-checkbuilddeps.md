# dpkg-checkbuilddeps command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-checkbuilddeps [<option>...] [<control-file>]

Options:
  -A             ignore Build-Depends-Arch and Build-Conflicts-Arch.
  -B             ignore Build-Depends-Indep and Build-Conflicts-Indep.
  -I             ignore built-in build dependencies and conflicts.
  -d build-deps  use given string as build dependencies instead of
                 retrieving them from control file
  -c build-conf  use given string for build conflicts instead of
                 retrieving them from control file
  -a arch        assume given host architecture
  -P profiles    assume given build profiles (comma-separated list)
  --admindir=<directory>
                 change the administrative directory.
  -?, --help     show this help message.
      --version  show the version.

<control-file> is the control file to process (default: debian/control).

~~~
