# sslyze command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: sslyze.py [options] target1.com target2.com:443 etc...

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  --xml_out=XML_FILE    Writes the scan results as an XML document to the file
                        XML_FILE. If XML_FILE is set to "-", the XML output
                        will instead be printed to stdout.
  --targets_in=TARGETS_IN
                        Reads the list of targets to scan from the file
                        TARGETS_IN. It should contain one host:port per line.
  --timeout=TIMEOUT     Sets the timeout value in seconds used for every
                        socket connection made to the target server(s).
                        Default is 5s.
  --nb_retries=NB_RETRIES
                        Sets the number retry attempts for all network
                        connections initiated throughout the scan. Increase
                        this value if you are getting a lot of
                        timeout/connection errors when scanning a specific
                        server. Decrease this value to increase the speed of
                        the scans; results may however return connection
                        errors. Default is 4 connection attempts.
  --https_tunnel=HTTPS_TUNNEL
                        Tunnels all traffic to the target server(s) through an
                        HTTP CONNECT proxy. HTTP_TUNNEL should be the proxy's
                        URL: 'http://USER:PW@HOST:PORT/'. For proxies
                        requiring authentication, only Basic Authentication is
                        supported.
  --starttls=STARTTLS   Performs StartTLS handshakes when connecting to the
                        target server(s). STARTTLS should be one of: ['smtp',
                        'xmpp', 'xmpp_server', 'pop3', 'ftp', 'imap', 'ldap',
                        'rdp', 'postgres', 'auto']. The 'auto' option will
                        cause SSLyze to deduce the protocol (ftp, imap, etc.)
                        from the supplied port number, for each target
                        servers.
  --xmpp_to=XMPP_TO     Optional setting for STARTTLS XMPP.  XMPP_TO should be
                        the hostname to be put in the 'to' attribute of the
                        XMPP stream. Default is the server's hostname.
  --sni=SNI             Use Server Name Indication to specify the hostname to
                        connect to. Will only affect TLS 1.0+ connections.
  --quiet               Hide script standard outputs. Will only affect script
                        output if --xml_out is set.
  --regular             Regular HTTPS scan; shortcut for --sslv2 --sslv3
                        --tlsv1 --tlsv1_1 --tlsv1_2 --reneg --resum
                        --certinfo=basic --http_get --hide_rejected_ciphers
                        --compression --heartbleed

  Client certificate support:
    --cert=CERT         Client certificate chain filename. The certificates
                        must be in PEM format and must be sorted starting with
                        the subject's client certificate, followed by
                        intermediate CA certificates if applicable.
    --key=KEY           Client private key filename.
    --keyform=KEYFORM   Client private key format. DER or PEM (default).
    --pass=KEYPASS      Client private key passphrase.

  PluginHSTS:
    --hsts              Checks support for HTTP Strict Transport Security
                        (HSTS) by collecting any Strict-Transport-Security
                        field present in the HTTP response sent back by the
                        server(s).

  PluginSessionResumption:
    Analyzes the target server's SSL session resumption capabilities.

    --resum             Tests the server(s) for session resumption support
                        using session IDs and TLS session tickets (RFC 5077).
    --resum_rate        Performs 100 session resumptions with the server(s),
                        in order to estimate the session resumption rate.

  PluginOpenSSLCipherSuites:
    Scans the server(s) for supported OpenSSL cipher suites.

    --sslv2             Lists the SSL 2.0 OpenSSL cipher suites supported by
                        the server(s).
    --sslv3             Lists the SSL 3.0 OpenSSL cipher suites supported by
                        the server(s).
    --tlsv1             Lists the TLS 1.0 OpenSSL cipher suites supported by
                        the server(s).
    --tlsv1_1           Lists the TLS 1.1 OpenSSL cipher suites supported by
                        the server(s).
    --tlsv1_2           Lists the TLS 1.2 OpenSSL cipher suites supported by
                        the server(s).
    --http_get          Option - For each cipher suite, sends an HTTP GET
                        request after completing the SSL handshake and returns
                        the HTTP status code.
    --hide_rejected_ciphers
                        Option - Hides the (usually long) list of cipher
                        suites that were rejected by the server(s).

  PluginHeartbleed:
    --heartbleed        Tests the server(s) for the OpenSSL Heartbleed
                        vulnerability (experimental).

  PluginChromeSha1Deprecation:
    --chrome_sha1       Determines if the server will be affected by Google
                        Chrome's SHA-1 deprecation plans. See
                        http://googleonlinesecurity.blogspot.com/2014/09
                        /gradually-sunsetting-sha-1.html for more information

  PluginCertInfo:
    --certinfo=CERTINFO
                        Verifies the validity of the server(s) certificate(s)
                        against various trust stores, checks for support for
                        OCSP stapling, and prints relevant fields of the
                        certificate. CERTINFO should be 'basic' or 'full'.
    --ca_file=CA_FILE   Local Certificate Authority file (in PEM format), to
                        verify the validity of the server(s) certificate(s)
                        against.

  PluginSessionRenegotiation:
    --reneg             Tests the server(s) for client-initiated renegotiation
                        and secure renegotiation support.

  PluginCompression:
    --compression       Tests the server(s) for Zlib compression support.

~~~
