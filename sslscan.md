# sslscan command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


[1;34m                   _
           ___ ___| |___  ___ __ _ _ __
          / __/ __| / __|/ __/ _` | '_ \
          \__ \__ \ \__ \ (_| (_| | | | |
          |___/___/_|___/\___\__,_|_| |_|

[0m
[1;34m		1.11.7-static
		OpenSSL 1.0.2i-dev  xx XXX xxxx
[0m[1;34mCommand:[0m
  [32msslscan [Options] [host:port | host][0m

[1;34mOptions:[0m
  [32m--targets=<file>[0m     A file containing a list of hosts to check.
                       Hosts can  be supplied  with ports (host:port)
  [32m--ipv4[0m               Only use IPv4
  [32m--ipv6[0m               Only use IPv6
  [32m--show-certificate[0m   Show full certificate information
  [32m--no-check-certificate[0m  Don't warn about weak certificate algorithm or keys
  [32m--show-client-cas[0m    Show trusted CAs for TLS client auth
  [32m--show-ciphers[0m       Show supported client ciphers
  [32m--show-cipher-ids[0m    Show cipher ids
  [32m--show-times[0m         Show handhake times in milliseconds
  [32m--ssl2[0m               Only check SSLv2 ciphers
  [32m--ssl3[0m               Only check SSLv3 ciphers
  [32m--tls10[0m              Only check TLSv1.0 ciphers
  [32m--tls11[0m              Only check TLSv1.1 ciphers
  [32m--tls12[0m              Only check TLSv1.2 ciphers
  [32m--tlsall[0m             Only check TLS ciphers (all versions)
  [32m--ocsp[0m               Request OCSP response from server
  [32m--pk=<file>[0m          A file containing the private key or a PKCS#12 file
                       containing a private key/certificate pair
  [32m--pkpass=<password>[0m  The password for the private  key or PKCS#12 file
  [32m--certs=<file>[0m       A file containing PEM/ASN1 formatted client certificates
  [32m--no-ciphersuites[0m    Do not check for supported ciphersuites
  [32m--no-fallback[0m        Do not check for TLS Fallback SCSV
  [32m--no-renegotiation[0m   Do not check for TLS renegotiation
  [32m--no-compression[0m     Do not check for TLS compression (CRIME)
  [32m--no-heartbleed[0m      Do not check for OpenSSL Heartbleed (CVE-2014-0160)
  [32m--starttls-ftp[0m       STARTTLS setup for FTP
  [32m--starttls-imap[0m      STARTTLS setup for IMAP
  [32m--starttls-irc[0m       STARTTLS setup for IRC
  [32m--starttls-pop3[0m      STARTTLS setup for POP3
  [32m--starttls-smtp[0m      STARTTLS setup for SMTP
  [32m--starttls-xmpp[0m      STARTTLS setup for XMPP
  [32m--starttls-psql[0m      STARTTLS setup for PostgreSQL
  [32m--xmpp-server[0m        Use a server-to-server XMPP handshake
  [32m--http[0m               Test a HTTP connection
  [32m--rdp[0m                Send RDP preamble before starting scan
  [32m--bugs[0m               Enable SSL implementation bug work-arounds
  [32m--timeout=<sec>[0m      Set socket timeout. Default is 3s
  [32m--sleep=<msec>[0m       Pause between connection request. Default is disabled
  [32m--xml=<file>[0m         Output results to an XML file
                       <file> can be -, which means stdout
  [32m--version[0m            Display the program version
  [32m--verbose[0m            Display verbose output
  [32m--no-cipher-details[0m  Disable EC curve names and EDH/RSA key lengths output
  [32m--no-colour[0m          Disable coloured output
  [32m--help[0m               Display the  help text  you are  now reading

[1;34mExample:[0m
  [32msslscan 127.0.0.1[0m
  [32msslscan [::1][0m


~~~
