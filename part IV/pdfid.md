# pdfid command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: pdfid [options] [pdf-file|zip-file|url|@file] ...
Tool to test a PDF file

Arguments:
pdf-file and zip-file can be a single file, several files, and/or @file
@file: run PDFiD on each file listed in the text file specified
wildcards are supported

Source code put in the public domain by Didier Stevens, no Copyright
Use at your own risk
https://DidierStevens.com

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -s, --scan            scan the given directory
  -a, --all             display all the names
  -e, --extra           display extra data, like dates
  -f, --force           force the scan of the file, even without proper %PDF
                        header
  -d, --disarm          disable JavaScript and auto launch
  -p PLUGINS, --plugins=PLUGINS
                        plugins to load (separate plugins with a comma , ;
                        @file supported)
  -c, --csv             output csv data when using plugins
  -m MINIMUMSCORE, --minimumscore=MINIMUMSCORE
                        minimum score for plugin results output
  -v, --verbose         verbose (will also raise catched exceptions)
  -S SELECT, --select=SELECT
                        selection expression
  -o OUTPUT, --output=OUTPUT
                        output to log file

~~~
