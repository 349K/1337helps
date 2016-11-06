# markdown_py command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: markdown_py [options] [INPUTFILE]
       (STDIN is assumed if no INPUTFILE is given)

A Python implementation of John Gruber's Markdown.
https://pythonhosted.org/Markdown/

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -f OUTPUT_FILE, --file=OUTPUT_FILE
                        Write output to OUTPUT_FILE. Defaults to STDOUT.
  -e ENCODING, --encoding=ENCODING
                        Encoding for input and output files.
  -s SAFE_MODE, --safe=SAFE_MODE
                        Deprecated! 'replace', 'remove' or 'escape' HTML tags
                        in input
  -o OUTPUT_FORMAT, --output_format=OUTPUT_FORMAT
                        'xhtml1' (default), 'html4' or 'html5'.
  -n, --no_lazy_ol      Observe number of first item of ordered lists.
  -x EXTENSION, --extension=EXTENSION
                        Load extension EXTENSION.
  -c CONFIG_FILE, --extension_configs=CONFIG_FILE
                        Read extension configurations from CONFIG_FILE.
                        CONFIG_FILE must be of JSON or YAML format. YAMLformat
                        requires that a python YAML library be installed. The
                        parsed JSON or YAML must result in a python dictionary
                        which would be accepted by the 'extension_configs'
                        keyword on the markdown.Markdown class. The extensions
                        must also be loaded with the `--extension` option.
  -q, --quiet           Suppress all warnings.
  -v, --verbose         Print all warnings.
  --noisy               Print debug messages.

~~~
