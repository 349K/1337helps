# dirmngr-client command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


dirmngr-client (GnuPG) 2.1.11
Copyright (C) 2016 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

Syntax: dirmngr-client [options] [certfile|pattern]
Test an X.509 certificate against a CRL or do an OCSP check
The process returns 0 if the certificate is valid, 1 if it is
not valid and other error codes for general failures

Options:
 -v, --verbose                   verbose
 -q, --quiet                     be somewhat more quiet
     --ocsp                      use OCSP instead of CRLs
     --ping                      check whether a dirmngr is running
     --cache-cert                add a certificate to the cache
     --validate                  validate a certificate
     --lookup                    lookup a certificate
 -l, --local                     lookup only locally stored certificates
 -u, --url                       expect an URL for --lookup
     --load-crl                  load a CRL into the dirmngr
     --squid-mode                special mode for use by Squid
     --pem                       expect certificates in PEM format
     --force-default-responder   force the use of the default OCSP responder

Please report bugs to <http://bugs.gnupg.org>.

~~~
