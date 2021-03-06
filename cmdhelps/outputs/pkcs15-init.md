# pkcs15-init command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: pkcs15-init [OPTIONS]
Options:
      --version                 Print OpenSC package version
  -E, --erase-card              Erase the smart card
  -C, --create-pkcs15           Creates a new PKCS #15 structure
  -P, --store-pin               Store a new PIN/PUK on the card
  -G, --generate-key <arg>      Generate a new key and store it on the card
  -S, --store-private-key <arg>
                                Store private key
      --store-public-key <arg>  Store public key
  -X, --store-certificate <arg>
                                Store an X.509 certificate
  -U, --update-certificate <arg>
                                Update an X.509 certificate (carefull with mail decryption certs!!)
  -W, --store-data <arg>        Store a data object
  -D, --delete-objects <arg>    Delete object(s) (use "help" for more information)
  -A, --change-attributes <arg>
                                Change attribute(s) (use "help" for more information)
      --sanity-check            Card specific sanity check and possibly update procedure
      --erase-application <arg>
                                Erase application with AID <arg>
  -r, --reader <arg>            Specify which reader to use
      --pin <arg>               Specify PIN
      --puk <arg>               Specify unblock PIN
      --so-pin <arg>            Specify security officer (SO) PIN
      --so-puk <arg>            Specify unblock PIN for SO PIN
      --no-so-pin               Do not install a SO PIN, and do not prompt for it
      --serial <arg>            Specify the serial number of the card
  -a, --auth-id <arg>           Specify ID of PIN to use/create
      --puk-id <arg>            Specify ID of PUK to use/create
      --verify-pin              Verify PIN after card binding (use with --auth-id)
  -i, --id <arg>                Specify ID of key/certificate
  -l, --label <arg>             Specify label of PIN/key
      --puk-label <arg>         Specify label of PUK
      --public-key-label <arg>  Specify public key label (use with --generate-key)
      --cert-label <arg>        Specify user cert label (use with --store-private-key)
      --application-name <arg>  Specify application name of data object (use with --store-data-object)
      --application-id <arg>    Specify application id of data object (use with --store-data-object)
      --aid <arg>               Specify AID of the on-card PKCS#15 application to be binded to (in hexadecimal form)
  -o, --output-file <arg>       Output public portion of generated key to file
  -f, --format <arg>            Specify key/cert file format: PEM (=default), DER or PKCS12
      --passphrase <arg>        Specify passphrase for unlocking secret key
      --authority               Mark certificate as a CA certificate
  -u, --key-usage <arg>         Specify X.509 key usage (use "--key-usage help" for more information)
  -F, --finalize                Finish initialization phase of the smart card
      --update-last-update      Update 'lastUpdate' attribut of tokenInfo
      --ignore-ca-certificates  When storing PKCS#12 ignore CA certificates
      --update-existing         Store or update existing certificate
      --extractable             Private key stored as an extractable key
      --insecure                Insecure mode: do not require a PIN for private key
  -T, --use-default-transport-keys
                                Do not ask for transport keys if the driver thinks it knows the key
      --no-prompt               Do not prompt the user; if no PINs supplied, pinpad will be used
  -p, --profile <arg>           Specify the general profile to use
  -c, --card-profile <arg>      Specify the card profile to use
      --options-file <arg>      Read additional command line options from file
      --md-container-guid <arg>
                                For a new key specify GUID for a MD container
  -w, --wait                    Wait for card insertion
  -h, --help                    Display this message
  -v, --verbose                 Verbose operation. Use several times to enable debug output.

~~~
