# dpkg-statoverride command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-statoverride [<option> ...] <command>

Commands:
  --add <owner> <group> <mode> <path>
                           add a new <path> entry into the database.
  --remove <path>          remove <path> from the database.
  --list [<glob-pattern>]  list current overrides in the database.

Options:
  --admindir <directory>   set the directory with the statoverride file.
  --update                 immediately update <path> permissions.
  --force                  force an action even if a sanity check fails.
  --quiet                  quiet operation, minimal output.
  --help                   show this help message.
  --version                show the version.


~~~
