# pkcs15-crypt command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: pkcs15-crypt [OPTIONS]
Options:
      --version                 Print OpenSC package version
  -s, --sign                    Performs digital signature operation
  -c, --decipher                Decipher operation
  -k, --key <arg>               Selects the private key ID to use
  -r, --reader <arg>            Uses reader number <arg>
  -i, --input <arg>             Selects the input file to use (defaults to stdin)
  -o, --output <arg>            Outputs to file <arg> (defaults to stdout)
  -f, --signature-format <arg>  Format for ECDSA signature <arg>: 'rs' (default), 'sequence', 'openssl'
  -R, --raw                     Outputs raw 8 bit data
      --sha-1                   Input file is a SHA-1 hash
      --sha-256                 Input file is a SHA-256 hash
      --sha-384                 Input file is a SHA-384 hash
      --sha-512                 Input file is a SHA-512 hash
      --sha-224                 Input file is a SHA-224 hash
      --md5                     Input file is a MD5 hash
      --pkcs1                   Use PKCS #1 v1.5 padding
  -p, --pin <arg>               Uses password (PIN) <arg> (use - for reading PIN from STDIN)
      --aid <arg>               Specify AID of the on-card PKCS#15 application to be binded to (in hexadecimal form)
  -w, --wait                    Wait for card insertion
  -v, --verbose                 Verbose operation. Use several times to enable debug output.

~~~
