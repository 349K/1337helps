# pathoc command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: pathoc [-h] [--show-uas] [--version] [-c HOST:PORT] [--memo-limit N]
              [-m] [-n N] [-w N] [-r] [-t TIMEOUT] [--http2]
              [--http2-skip-connection-preface] [-s] [-C CLIENTCERT] [-i SNI]
              [--ciphers CIPHERS]
              [--ssl-version {all,TLSv1_2,secure,TLSv1_1,TLSv1,SSLv3,SSLv2}]
              [-I IGNORECODES] [-S] [-e] [-o] [-q] [-p] [-T] [-x]
              [--http2-framedump]
              host[:port] requests [requests ...]

A perverse HTTP client.

positional arguments:
  host[:port]           Host and port to connect to
  requests              Request specification, or path to a file containing
                        request specifcations

optional arguments:
  -h, --help            show this help message and exit
  --show-uas            Print user agent shortcuts and exit.
  --version             show program's version number and exit
  -c HOST:PORT          Issue an HTTP CONNECT to connect to the specified
                        host.
  --memo-limit N        Stop if we do not find a valid request after N
                        attempts.
  -m                    Remember specs, and never play the same one twice.
                        Note that this means requests have to be rendered in
                        memory, which means that large generated data can
                        cause issues.
  -n N                  Repeat N times. If 0 repeat for ever.
  -w N                  Wait N seconds between each request.
  -r                    Select a random request from those specified. If this
                        is not specified, requests are all played in sequence.
  -t TIMEOUT            Connection timeout
  --http2               Perform all requests over a single HTTP/2 connection.
  --http2-skip-connection-preface
                        Skips the HTTP/2 connection preface before sending
                        requests.

SSL:
  -s                    Connect with SSL
  -C CLIENTCERT         Path to a file containing client certificate and
                        private key
  -i SNI                SSL Server Name Indication
  --ciphers CIPHERS     SSL cipher specification
  --ssl-version {all,TLSv1_2,secure,TLSv1_1,TLSv1,SSLv3,SSLv2}
                        Set supported SSL/TLS versions. SSLv2, SSLv3 and 'all'
                        are INSECURE. Defaults to secure, which is TLS1.0+.

Controlling Output:
  Some of these options expand generated values for logging - if you're
  generating large data, use them with caution.

  -I IGNORECODES        Comma-separated list of response codes to ignore
  -S                    Show info on SSL connection
  -e                    Explain requests
  -o                    Oneshot - exit after first non-ignored response
  -q                    Print full request
  -p                    Print full response
  -T                    Ignore timeouts
  -x                    Output in hexdump format
  --http2-framedump     Output all received & sent HTTP/2 frames

~~~
