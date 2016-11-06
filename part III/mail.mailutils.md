# mail.mailutils command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: mail.mailutils [OPTION...] [address...]
  or:  mail.mailutils [OPTION...] -f [OPTION...] [file]
  or:  mail.mailutils [OPTION...] --file [OPTION...] [file]
  or:  mail.mailutils [OPTION...] --file=file [OPTION...]
GNU mail -- process mail messages.
If -f or --file is given, mail operates on the mailbox named by the first
argument, or the user's mbox, if no argument given.

  -a, --append=HEADER: VALUE append given header to the message being sent
  -A, --attach=FILE          attach FILE
      --content-type=TYPE    set content type for subsequent --attach options
  -e, --exist                return true if mail exists
      --encoding=NAME        set encoding for subsequent --attach options
  -E, --exec=COMMAND         execute COMMAND
  -F, --byname               save messages according to sender
  -H, --headers              write a header summary and exit
  -i, --ignore               ignore interrupts
  -n, --norc                 do not read the system mailrc file
  -N, --nosum                do not display initial header summary
  -p, --print, --read        print all mail to standard output
  -q, --quit                 cause interrupts to terminate program
  -r, --return-address=ADDRESS   use address as the return address when sending
                             mail
  -s, --subject=SUBJ         send a message with the given SUBJECT
  -t, --to                   precede message by a list of addresses
  -u, --user=USER            operate on USER's mailbox

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

Report bugs to: <bug-mailutils@gnu.org>
GNU Mailutils home page: <http://mailutils.org>
General help using GNU software: <http://www.gnu.org/gethelp/>

~~~
