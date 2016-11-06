# apt-mark command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

apt 1.3.1 (amd64)
Usage: apt-mark [options] {auto|manual} pkg1 [pkg2 ...]

apt-mark is a simple command line interface for marking packages
as manually or automatically installed. It can also be used to
manipulate the dpkg(1) selection states of packages, and to list
all packages with or without a certain marking.

Most used commands:
  auto - Mark the given packages as automatically installed
  manual - Mark the given packages as manually installed
  hold - Mark a package as held back
  unhold - Unset a package set as held back
  showauto - Print the list of automatically installed packages
  showmanual - Print the list of manually installed packages
  showhold - Print the list of package on hold

See apt-mark(8) for more information about the available commands.
Configuration options and syntax is detailed in apt.conf(5).
Information about how to configure sources can be found in sources.list(5).
Package and version choices can be expressed via apt_preferences(5).
Security details are available in apt-secure(8).

~~~
