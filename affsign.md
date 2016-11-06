# affsign command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

affsign version 3.7.10
usage: affsign [options] filename.aff
This program will:
  * Sign each segment if there are no segment signatures.
  * Write signed chain-of-custody Bill of Materials segment.

Signature Options:
   -k filename.key   = specify private key for signing
   -c filename.cer   = specify a X.509 certificate that matches the private key
                       (by default, the file is assumed to be the same one
                       provided with the -k option.)
   -Z                = ZAP (remove) all signature segments.
options:
    -n      --- ask for a chain-of-custody note.
    -v      --- Just print the version number and exit.

~~~
