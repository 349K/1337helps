# sieve command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: sieve [OPTION...] SCRIPT
GNU sieve -- a mail filtering tool.

  -c, --compile-only         compile script and exit
  -d, --debug[=FLAGS]        debug flags (defaults to "TPt")
  -D, --dump                 compile script, dump disassembled sieve code to
                             terminal and exit
  -e, --email=ADDRESS        override user email address
  -E, --expression           treat SCRIPT as Sieve program text
  -f, --mbox-url=MBOX        mailbox to sieve (defaults to user's mail spool)
  -k, --keep-going           keep on going if execution fails on a message
      --line-info[=BOOL]     print source location along with action logs
                             (default)
  -n, --no-actions, --dry-run   do not execute any actions, just print what
                             would be done
      --no-program-name      do not prefix diagnostic messages with the program
                             name
  -t, --ticket=TICKET        ticket file for user authentication
  -v, --verbose              log all actions

 Sieve options
      --clear-include-path   clear Sieve include path
      --clear-library-path, --clearpath
                             clear Sieve library path
  -I, --includedir=DIR       append DIR to the list of directories searched for
                             include files
      --libdir-prefix=DIR    add DIR to the beginning of the list of
                             directories searched for library files
  -L, --libdir=DIR           append DIR to the list of directories searched for
                             library files

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
      --log-facility=FACILITY   output logs to syslog FACILITY
  -M, --mailer=MAILER        use specified URL as the default mailer

  -?, --help                 give this help list
      --usage                give a short usage message
  -V, --version              print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

Debug flags:
  g - main parser traces
  T - mailutils traces (same as --debug-level=sieve.trace0-trace1)
  P - network protocols (same as --debug-level=sieve.=prot)
  t - sieve trace (MU_SIEVE_DEBUG_TRACE)
  i - sieve instructions trace (MU_SIEVE_DEBUG_INSTR)

Report bugs to: <bug-mailutils@gnu.org>
GNU Mailutils home page: <http://mailutils.org>
General help using GNU software: <http://www.gnu.org/gethelp/>

~~~
