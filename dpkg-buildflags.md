# dpkg-buildflags command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-buildflags [<command>]

Commands:
  --get <flag>       output the requested flag to stdout.
  --origin <flag>    output the origin of the flag to stdout:
                     value is one of vendor, system, user, env.
  --query-features <area>
                     output the status of features for the given area.
  --list             output a list of the flags supported by the current vendor.
  --export=(sh|make|cmdline|configure)
                     output something convenient to import the compilation
                     flags in a shell script, in make, or in a command line.
  --dump             output all compilation flags with their values
  --status           print a synopsis with all parameters affecting the
                     behaviour of dpkg-buildflags and the resulting flags
                     and their origin.
  --help             show this help message.
  --version          show the version.

~~~
