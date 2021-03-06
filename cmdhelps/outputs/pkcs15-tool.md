# pkcs15-tool command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: pkcs15-tool [OPTIONS]
Options:
      --version                 Print OpenSC package version
  -L, --learn-card              Stores card info to cache
      --list-applications       List the on-card PKCS#15 applications
  -r, --read-certificate <arg>  Reads certificate with ID <arg>
  -c, --list-certificates       Lists certificates
  -R, --read-data-object <arg>  Reads data object with OID, applicationName or label <arg>
      --raw                     Outputs raw 8 bit data to stdout. File output will not be affected by this, it always uses raw mode.
  -C, --list-data-objects       Lists data objects
      --list-pins               Lists PIN codes
      --list-secret-keys        Lists secret keys
  -D, --dump                    Dump card objects
  -u, --unblock-pin             Unblock PIN code
      --change-pin              Change PIN or PUK code
  -k, --list-keys               Lists private keys
      --list-public-keys        Lists public keys
      --read-public-key <arg>   Reads public key with ID <arg>
      --read-ssh-key <arg>      Reads public key with ID <arg>, outputs ssh format
      --rfc4716                 Outputs the public key in RFC 4716 format (requires --read-ssh-key)
  -T, --test-update             Test if the card needs a security update
  -U, --update                  Update the card with a security update
      --reader <arg>            Uses reader number <arg>
      --pin <arg>               Specify PIN
      --new-pin <arg>           Specify New PIN (when changing or unblocking)
      --puk <arg>               Specify Unblock PIN
      --verify-pin              Verify PIN after card binding (without 'auth-id' the first non-SO, non-Unblock PIN will be verified)
  -o, --output <arg>            Outputs to file <arg>
      --no-cache                Disable card caching
  -a, --auth-id <arg>           The auth ID of the PIN to use
      --aid <arg>               Specify AID of the on-card PKCS#15 application to bind to (in hexadecimal form)
  -w, --wait                    Wait for card insertion
  -v, --verbose                 Verbose operation. Use several times to enable debug output.
      --no-prompt               Do not prompt the user; if no PINs supplied, pinpad will be used.

~~~
