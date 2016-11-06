# dpkg-trigger command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-trigger [<options> ...] <trigger-name>
       dpkg-trigger [<options> ...] <command>

Commands:
  --check-supported                Check if the running dpkg supports triggers.

  -?, --help                       Show this help message.
      --version                    Show the version.

Options:
  --admindir=<directory>           Use <directory> instead of /var/lib/dpkg.
  --by-package=<package>           Override trigger awaiter (normally set
                                     by dpkg).
  --await                          Package needs to await the processing.
  --no-await                       No package needs to await the processing.
  --no-act                         Just test - don't actually change anything.


~~~
