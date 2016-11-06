# mako-render command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: usage: %prog [FILENAME] [-h] [--var VAR] [--template-dir TEMPLATE_DIR]
                               [input]

positional arguments:
  input

optional arguments:
  -h, --help            show this help message and exit
  --var VAR             variable (can be used multiple times, use name=value)
  --template-dir TEMPLATE_DIR
                        Directory to use for template lookup (multiple
                        directories may be provided). If not given then if the
                        template is read from stdin, the value defaults to be
                        the current directory, otherwise it defaults to be the
                        parent directory of the file provided.

~~~
