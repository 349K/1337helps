# zim command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: zim [OPTIONS] [NOTEBOOK [PAGE]]
   or: zim --server [OPTIONS] [NOTEBOOK]
   or: zim --export [OPTIONS] NOTEBOOK [PAGE]
   or: zim --search NOTEBOOK QUERY
   or: zim --index  NOTEBOOK
   or: zim --plugin PLUGIN [ARGUMENTS]
   or: zim --manual [OPTIONS] [PAGE]
   or: zim --help

General Options:
  --gui            run the editor (this is the default)
  --server         run the web server
  --export         export to a different format
  --search         run a search query on a notebook
  --index          build an index for a notebook
  --plugin         call a specific plugin function
  --manual         open the user manual
  -V, --verbose    print information to terminal
  -D, --debug      print debug messages
  -v, --version    print version and exit
  -h, --help       print this text

GUI Options:
  --list           show the list with notebooks instead of
                   opening the default notebook
  --geometry       window size and position as WxH+X+Y
  --fullscreen     start in fullscreen mode
  --standalone     start a single instance, no background process

Server Options:
  --port           port to use (defaults to 8080)
  --template       name of the template to use
  --gui            run the gui wrapper for the server

Export Options:
  -o, --output     output directory (mandatory option)
  --format         format to use (defaults to 'html')
  --template       name of the template to use
  --root-url       url to use for the document root
  --index-page     index page name
  -r, --recursive  when exporting a page, also export sub-pages
  -s, --singlefile export all pages to a single output file
  -O, --overwrite  force overwriting existing file(s)

Search Options:
  None

Index Options:
  None

Try 'zim --manual' for more help.


~~~
