# mimeview command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: mimeview [OPTION...] FILE [FILE ...]
GNU mimeview -- display files, using mailcap mechanism.

  -a, --no-ask[=TYPE-LIST]   do not ask for confirmation before displaying
                             files, or, if TYPE-LIST is given, do not ask for
                             confirmation before displaying such files whose
                             MIME type matches one of the patterns from
                             TYPE-LIST
  -d, --debug[=FLAGS]        enable debugging output
  -h, --no-interactive, --print   disable interactive mode
      --metamail[=FILE]      use metamail to display files
  -n, --dry-run              do not do anything, just print what whould be
                             done
  -t, --mimetypes=FILE       use this mime.types file

 Common options
      --config-file=FILE, --rcfile=FILE
                             load this configuration file
      --config-help          show configuration file summary
      --config-lint, --rcfile-lint
                             check configuration file syntax and exit
      --config-verbose, --rcfile-verbose
                             verbosely log parsing of the configuration files
      --no-site-config, --no-site-rcfile
                             do not load site configuration file
      --no-user-config, --no-user-rcfile
                             do not load user configuration file
      --set=PARAM=VALUE      set configuration parameter
      --show-config-options  show compilation options


 Global debugging settings
      --debug-level=LEVEL    set Mailutils debugging level
      --debug-line-info      show source info with debugging messages

  -?, --help                 give this help list
      --usage                give a short usage message
  -V, --version              print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

Default mime.types file is /usr/share/cups/mime/mime.types

Debug flags are:
  g - Mime.types parser traces
  l - Mime.types lexical analyzer traces
  0-9 - Set debugging level

Report bugs to: <bug-mailutils@gnu.org>
GNU Mailutils home page: <http://mailutils.org>
General help using GNU software: <http://www.gnu.org/gethelp/>

~~~
