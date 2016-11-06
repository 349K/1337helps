# vbutil_key command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:  futility vbutil_key --pack <outfile> [PARAMETERS]

  Required parameters:
    --key <infile>              RSA key file (.keyb or .pem)
    --version <number>          Key version number (required for .keyb,
                                  ignored for .pem)
    --algorithm <number>        Signing algorithm to use with key:
                                  0 = (RSA1024 SHA1)
                                  1 = (RSA1024 SHA256)
                                  2 = (RSA1024 SHA512)
                                  3 = (RSA2048 SHA1)
                                  4 = (RSA2048 SHA256)
                                  5 = (RSA2048 SHA512)
                                  6 = (RSA4096 SHA1)
                                  7 = (RSA4096 SHA256)
                                  8 = (RSA4096 SHA512)
                                  9 = (RSA8192 SHA1)
                                  10 = (RSA8192 SHA256)
                                  11 = (RSA8192 SHA512)

OR

Usage:  futility vbutil_key --unpack <infile>

  Optional parameters:
    --copyto <file>             Write a copy of the key to this file.


~~~
