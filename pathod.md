# pathod command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: pathod [-h] [--version] [-p PORT] [-l ADDRESS] [-a ANCHOR]
              [-c CRAFTANCHOR] [--confdir CONFDIR] [-d STATICDIR] [-D]
              [-t TIMEOUT] [--limit-size SIZELIMIT] [--noapi] [--nohang]
              [--noweb] [--nocraft] [--webdebug] [-s] [--cn CN] [-C]
              [--cert SPEC] [--ciphers CIPHERS] [--san SAN]
              [--ssl-version {all,TLSv1_2,secure,TLSv1_1,TLSv1,SSLv3,SSLv2}]
              [-e] [-f LOGFILE] [-q] [-r] [-x] [--http2-framedump]

A pathological HTTP/S daemon.

optional arguments:
  -h, --help            show this help message and exit
  --version             show program's version number and exit
  -p PORT               Port. Specify 0 to pick an arbitrary empty port.
                        (9999)
  -l ADDRESS            Listening address. (127.0.0.1)
  -a ANCHOR             Add an anchor. Specified as a string with the form
                        pattern=spec or pattern=filepath, where pattern is a
                        regular expression.
  -c CRAFTANCHOR        URL path specifying prefix for URL crafting commands.
                        (/p/)
  --confdir CONFDIR     Configuration directory. (~/.mitmproxy)
  -d STATICDIR          Directory for static files.
  -D                    Daemonize.
  -t TIMEOUT            Connection timeout
  --limit-size SIZELIMIT
                        Size limit of served responses. Understands size
                        suffixes, i.e. 100k.
  --noapi               Disable API.
  --nohang              Disable pauses during crafted response generation.
  --noweb               Disable both web interface and API.
  --nocraft             Disable response crafting. If anchors are specified,
                        they still work.
  --webdebug            Debugging mode for the web app (dev only).

SSL:
  -s                    Run in HTTPS mode.
  --cn CN               CN for generated SSL certs. Default: pathod.net
  -C                    Don't expect SSL after a CONNECT request.
  --cert SPEC           Add an SSL certificate. SPEC is of the form
                        "[domain=]path". The domain may include a wildcard,
                        and is equal to "*" if not specified. The file at path
                        is a certificate in PEM format. If a private key is
                        included in the PEM, it is used, else the default key
                        in the conf dir is used. Can be passed multiple times.
  --ciphers CIPHERS     SSL cipher specification
  --san SAN             Subject Altnernate Name to add to the server
                        certificate. May be passed multiple times.
  --ssl-version {all,TLSv1_2,secure,TLSv1_1,TLSv1,SSLv3,SSLv2}
                        Set supported SSL/TLS versions. SSLv2, SSLv3 and 'all'
                        are INSECURE. Defaults to secure, which is TLS1.0+.

Controlling Logging:
  Some of these options expand generated values for logging - if you're
  generating large data, use them with caution.

  -e                    Explain responses
  -f LOGFILE            Log to file.
  -q                    Log full request
  -r                    Log full response
  -x                    Log request/response in hexdump format
  --http2-framedump     Output all received & sent HTTP/2 frames

~~~
