# svnmucc command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: svnmucc ACTION...
Subversion multiple URL command client.
Type 'svnmucc --version' to see the program version and RA modules.

  Perform one or more Subversion repository URL-based ACTIONs, committing
  the result as a (single) new revision.

Actions:
  cp REV SRC-URL DST-URL : copy SRC-URL@REV to DST-URL
  mkdir URL              : create new directory URL
  mv SRC-URL DST-URL     : move SRC-URL to DST-URL
  rm URL                 : delete URL
  put SRC-FILE URL       : add or modify file URL with contents copied from
                           SRC-FILE (use "-" to read from standard input)
  propset NAME VALUE URL : set property NAME on URL to VALUE
  propsetf NAME FILE URL : set property NAME on URL to value read from FILE
  propdel NAME URL       : delete property NAME from URL

Valid options:
  -h, -? [--help]        : display this text
  -m [--message] ARG     : use ARG as a log message
  -F [--file] ARG        : read log message from file ARG
  -u [--username] ARG    : commit the changes as username ARG
  -p [--password] ARG    : use ARG as the password
  -U [--root-url] ARG    : interpret all action URLs relative to ARG
  -r [--revision] ARG    : use revision ARG as baseline for changes
  --with-revprop ARG     : set revision property in the following format:
                               NAME[=VALUE]
  --non-interactive      : do no interactive prompting (default is to
                           prompt only if standard input is a terminal)
  --force-interactive    : do interactive prompting even if standard
                           input is not a terminal
  --trust-server-cert    : deprecated;
                           same as --trust-server-cert-failures=unknown-ca
  --trust-server-cert-failures ARG
                           with --non-interactive, accept SSL server
                           certificates with failures; ARG is comma-separated
                           list of 'unknown-ca' (Unknown Authority),
                           'cn-mismatch' (Hostname mismatch), 'expired'
                           (Expired certificate),'not-yet-valid' (Not yet
                           valid certificate) and 'other' (all other not
                           separately classified certificate errors).
  -X [--extra-args] ARG  : append arguments from file ARG (one per line;
                           use "-" to read from standard input)
  --config-dir ARG       : use ARG to override the config directory
  --config-option ARG    : use ARG to override a configuration option
  --no-auth-cache        : do not cache authentication tokens
  --version              : print version information

~~~
