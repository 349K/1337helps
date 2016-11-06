# ndg_httpclient command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: ndg_httpclient [options] url

Options:
  -h, --help            show this help message and exit
  -c FILE, --certificate=FILE
                        Certificate file - defaults to $HOME/credentials.pem
  -k FILE, --private-key=FILE
                        Private key file - defaults to the certificate file
  -t PATH, --ca-certificate-dir=PATH
                        Trusted CA certificate file directory
  -d, --debug           Print debug information.
  -p FILE, --post-data-file=FILE
                        POST data file
  -f FILE, --fetch=FILE
                        Output file
  -n, --no-verify-peer  Skip verification of peer certificate.
  -a USER:PASSWD, --basicauth=USER:PASSWD
                        HTTP authentication credentials
  --header=HEADER: VALUE
                        Add HTTP header to request

~~~
