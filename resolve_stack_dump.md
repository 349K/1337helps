# resolve_stack_dump command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

resolve_stack_dump  Ver 1.5 Distrib 5.6.30, for debian-linux-gnu (x86_64)
Copyright (c) 2001, 2016, Oracle and/or its affiliates. All rights reserved.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Resolve numeric stack strace dump into symbols.

Usage: resolve_stack_dump [OPTIONS] symbols-file [numeric-dump-file]
  -h, --help          Display this help and exit.
  -V, --version       Output version information and exit.
  -s, --symbols-file=name 
                      Use specified symbols file.
  -n, --numeric-dump-file=name 
                      Read the dump from specified file.

Variables (--variable-name=value)
and boolean options {FALSE|TRUE}  Value (after reading options)
--------------------------------- ----------------------------------------
symbols-file                      (No default value)
numeric-dump-file                 (No default value)

The symbols-file should include the output from:  'nm --numeric-sort mysqld'.
The numeric-dump-file should contain a numeric stack trace from mysqld.
If the numeric-dump-file is not given, the stack trace is read from stdin.

~~~
