# dirmngr command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


dirmngr (GnuPG) 2.1.11
Copyright (C) 2016 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

Syntax: dirmngr [options] [command [args]]
Keyserver, CRL, and OCSP access for GnuPG

Commands:
 
     --server                     run in server mode (foreground)
     --daemon                     run in daemon mode (background)
     --list-crls                  list the contents of the CRL cache
     --load-crl FILE              load CRL from FILE into cache
     --fetch-crl URL              fetch a CRL from URL
     --shutdown                   shutdown the dirmngr
     --flush                      flush the cache

Options:
 
 -v, --verbose                    verbose
 -q, --quiet                      be somewhat more quiet
 -s, --sh                         sh-style command output
 -c, --csh                        csh-style command output
     --options FILE               read options from FILE
     --debug-level LEVEL          set the debugging level to LEVEL
     --no-detach                  do not detach from the console
     --log-file FILE              write server mode logs to FILE
     --batch                      run without asking a user
     --force                      force loading of outdated CRLs
     --allow-ocsp                 allow sending OCSP requests
     --disable-http               inhibit the use of HTTP
     --disable-ldap               inhibit the use of LDAP
     --ignore-http-dp             ignore HTTP CRL distribution points
     --ignore-ldap-dp             ignore LDAP CRL distribution points
     --ignore-ocsp-service-url    ignore certificate contained OCSP service URLs
     --http-proxy URL             redirect all HTTP requests to URL
     --ldap-proxy HOST            use HOST for LDAP queries
     --only-ldap-proxy            do not use fallback hosts with --ldap-proxy
     --ldapserverlist-file FILE   read LDAP server list from FILE
     --add-servers                add new servers discovered in CRL distribution points to serverlist
     --ldaptimeout N              set LDAP timeout to N seconds
     --ocsp-responder URL         use OCSP responder at URL
     --ocsp-signer FPR            OCSP response signed by FPR
     --max-replies N              do not return more than N items in one query
     --hkp-cacert FILE            use the CA certificates in FILE for HKP over TLS
     --use-tor                    route all network traffic via Tor

(See the "info" manual for a complete listing of all commands and options)

Please report bugs to <http://bugs.gnupg.org>.

~~~
