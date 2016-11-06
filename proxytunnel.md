# proxytunnel command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

proxytunnel 1.9.0 (rev 242) Copyright 2001-2008 Proxytunnel Project
Usage: proxytunnel [OPTIONS]...
Build generic tunnels trough HTTPS proxies using HTTP authentication

Standard options:
 -i, --inetd               Run from inetd (default: off)
 -a, --standalone=INT      Run as standalone daemon on specified port
 -p, --proxy=STRING        Local proxy host:port combination
 -r, --remproxy=STRING     Remote proxy host:port combination (using 2 proxies)
 -d, --dest=STRING         Destination host:port combination
 -e, --encrypt             SSL encrypt data between local proxy and destination
 -E, --encrypt-proxy       SSL encrypt data between client and local proxy
 -X, --encrypt-remproxy    SSL encrypt data between local and remote proxy
 -W, --wa-bug-29744        Workaround ASF Bugzilla 29744: if SSL is active stop
                           using it after CONNECT (might not work on all setups; see
                           /usr/share/doc/proxytunnel/README.Debian.gz)
 -B, --buggy-encrypt-proxy Equivalent to -E -W, provided for backwards
                           compatibility

Additional options for specific features:
 -F, --passfile=STRING     File with credentials for proxy authentication
 -P, --proxyauth=STRING    Proxy auth credentials user:pass combination
 -R, --remproxyauth=STRING Remote proxy auth credentials user:pass combination
 -N, --ntlm                Use NTLM based authentication
 -t, --domain=STRING       NTLM domain (default: autodetect)
 -H, --header=STRING       Add additional HTTP headers to send to proxy
 -x, --proctitle=STRING    Use a different process title

Miscellaneous options:
 -v, --verbose             Turn on verbosity
 -q, --quiet               Suppress messages
 -h, --help                Print help and exit
 -V, --version             Print version and exit

~~~
