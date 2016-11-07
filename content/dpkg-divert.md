# dpkg-divert command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-divert [<option> ...] <command>

Commands:
  [--add] <file>           add a diversion.
  --remove <file>          remove the diversion.
  --list [<glob-pattern>]  show file diversions.
  --listpackage <file>     show what package diverts the file.
  --truename <file>        return the diverted file.

Options:
  --package <package>      name of the package whose copy of <file> will not
                             be diverted.
  --local                  all packages' versions are diverted.
  --divert <divert-to>     the name used by other packages' versions.
  --rename                 actually move the file aside (or back).
  --admindir <directory>   set the directory with the diversions file.
  --test                   don't do anything, just demonstrate.
  --quiet                  quiet operation, minimal output.
  --help                   show this help message.
  --version                show the version.

When adding, default is --local and --divert <original>.distrib.
When removing, --package or --local and --divert must match if specified.
Package preinst/postrm scripts should always specify --package and --divert.

~~~
