# apt-cache command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

apt 1.3.1 (amd64)
Usage: apt-cache [options] command
       apt-cache [options] show pkg1 [pkg2 ...]

apt-cache queries and displays available information about installed
and installable packages. It works exclusively on the data acquired
into the local cache via the 'update' command of e.g. apt-get. The
displayed information may therefore be outdated if the last update was
too long ago, but in exchange apt-cache works independently of the
availability of the configured sources (e.g. offline).

Most used commands:
  showsrc - Show source records
  search - Search the package list for a regex pattern
  depends - Show raw dependency information for a package
  rdepends - Show reverse dependency information for a package
  show - Show a readable record for the package
  pkgnames - List the names of all packages in the system
  policy - Show policy settings

See apt-cache(8) for more information about the available commands.
Configuration options and syntax is detailed in apt.conf(5).
Information about how to configure sources can be found in sources.list(5).
Package and version choices can be expressed via apt_preferences(5).
Security details are available in apt-secure(8).

~~~
