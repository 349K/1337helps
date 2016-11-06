# cryptoflex-tool command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: cryptoflex-tool [OPTIONS]
Options:
  -l, --list-keys               Lists all keys in a public key file
  -c, --create-key-files <arg>  Creates new RSA key files for <arg> keys
  -P, --create-pin-file <arg>   Creates a new CHV<arg> file
  -g, --generate-key            Generates a new RSA key pair
  -R, --read-key                Reads a public key from the card
  -V, --verify-pin              Verifies CHV1 before issuing commands
  -k, --key-num <arg>           Selects which key number to operate on [1]
  -a, --app-df <arg>            Selects the DF to operate in
  -p, --prkey-file <arg>        Private key file
  -u, --pubkey-file <arg>       Public key file
  -e, --exponent <arg>          The RSA exponent to use in key generation [3]
  -m, --modulus-length <arg>    Modulus length to use in key generation [1024]
  -r, --reader <arg>            Uses reader <arg>
  -w, --wait                    Wait for card insertion
  -v, --verbose                 Verbose operation. Use several times to enable debug output.

~~~
