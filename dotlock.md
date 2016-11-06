# dotlock command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dotlock [OPTION...] FILE
GNU dotlock -- lock mail spool files.

  -d, --debug                print details of failure reasons to stderr
  -f, --force[=MINUTES]      forcibly break an existing lock older than a
                             certain time
  -r, --retry[=RETRIES]      retry the lock a few times
  -u, --unlock               unlock

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

Returns 0 on success, 3 if locking the file fails because it's already locked,
and 1 if some other kind of error occurred.

Report bugs to: <bug-mailutils@gnu.org>
GNU Mailutils home page: <http://mailutils.org>
General help using GNU software: <http://www.gnu.org/gethelp/>

~~~
