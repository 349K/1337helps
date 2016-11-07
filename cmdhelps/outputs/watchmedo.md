# watchmedo command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: watchmedo [-h] [--version]
                 {tricks-from,tricks-generate-yaml,log,shell-command,auto-restart}
                 ...

positional arguments:
  {tricks-from,tricks-generate-yaml,log,shell-command,auto-restart}
    tricks-from         Subcommand to execute tricks from a tricks
                        configuration file. :param args: Command line argument
                        options.
    tricks-generate-yaml
                        Subcommand to generate Yaml configuration for tricks
                        named on the command line. :param args: Command line
                        argument options.
    log                 Subcommand to log file system events to the console.
                        :param args: Command line argument options.
    shell-command       Subcommand to execute shell commands in response to
                        file system events. :param args: Command line argument
                        options.
    auto-restart        Subcommand to start a long-running subprocess and
                        restart it on matched events. :param args: Command
                        line argument options.

optional arguments:
  -h, --help            show this help message and exit
  --version             show program's version number and exit

Copyright 2011 Yesudeep Mangalapilly <yesudeep@gmail.com>.
Copyright 2012 Google, Inc.

Licensed under the terms of the Apache license, version 2.0. Please see
LICENSE in the source code for more information.

~~~
