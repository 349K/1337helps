# pkcs11-tool command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: pkcs11-tool [OPTIONS]
Options:
      --module <arg>            Specify the module to load (default:opensc-pkcs11.so)
  -I, --show-info               Show global token information
  -L, --list-slots              List available slots
  -T, --list-token-slots        List slots with tokens
  -M, --list-mechanisms         List mechanisms supported by the token
  -O, --list-objects            Show objects on token
  -s, --sign                    Sign some data
      --decrypt                 Decrypt some data
  -h, --hash                    Hash some data
      --derive                  Derive a secret key using another key and some data
  -m, --mechanism <arg>         Specify mechanism (use -M for a list of supported mechanisms)
  -l, --login                   Log into the token first
      --login-type <arg>        Specify login type ('so', 'user', 'context-specific'; default:'user')
  -p, --pin <arg>               Supply User PIN on the command line (if used in scripts: careful!)
      --puk <arg>               Supply User PUK on the command line
      --new-pin <arg>           Supply new User PIN on the command line
      --so-pin <arg>            Supply SO PIN on the command line (if used in scripts: careful!)
      --init-token              Initialize the token, its label and its SO PIN (use with --label and --so-pin)
      --init-pin                Initialize the User PIN (use with --pin and --login)
  -c, --change-pin              Change User PIN
      --unlock-pin              Unlock User PIN (without '--login' unlock in logged in session; otherwise '--login-type' has to be 'context-specific')
  -k, --keypairgen              Key pair generation
      --key-type <arg>          Specify the type and length of the key to create, for example rsa:1024 or EC:prime256v1
      --usage-sign              Specify 'sign' key usage flag (sets SIGN in privkey, sets VERIFY in pubkey)
      --usage-decrypt           Specify 'decrypt' key usage flag (RSA only, set DECRYPT privkey, ENCRYPT in pubkey)
      --usage-derive            Specify 'derive' key usage flag (EC only)
  -w, --write-object <arg>      Write an object (key, cert, data) to the card
  -r, --read-object             Get object's CKA_VALUE attribute (use with --type)
  -b, --delete-object           Delete an object
      --application-label <arg>
                                Specify the application label of the data object (use with --type data)
      --application-id <arg>    Specify the application ID of the data object (use with --type data)
      --issuer <arg>            Specify the issuer in hexadecimal format (use with --type cert)
      --subject <arg>           Specify the subject in hexadecimal format (use with --type cert/privkey/pubkey)
  -y, --type <arg>              Specify the type of object (e.g. cert, privkey, pubkey, data)
  -d, --id <arg>                Specify the ID of the object
  -a, --label <arg>             Specify the label of the object
      --slot <arg>              Specify the ID of the slot to use
      --slot-description <arg>  Specify the description of the slot to use
      --slot-index <arg>        Specify the index of the slot to use
      --token-label <arg>       Specify the token label of the slot to use
  -e, --set-id <arg>            Set the CKA_ID of an object, <args>= the (new) CKA_ID
      --attr-from <arg>         Use <arg> to create some attributes when writing an object
  -i, --input-file <arg>        Specify the input file
  -o, --output-file <arg>       Specify the output file
  -f, --signature-format <arg>  Format for ECDSA signature <arg>: 'rs' (default), 'sequence', 'openssl'
  -t, --test                    Test (best used with the --login or --pin option)
      --test-hotplug            Test hotplug capabilities (C_GetSlotList + C_WaitForSlotEvent)
  -z, --moz-cert <arg>          Test Mozilla-like keypair gen and cert req, <arg>=certfile
  -v, --verbose                 Verbose operation. (Set OPENSC_DEBUG to enable OpenSC specific debugging)
      --private                 Set the CKA_PRIVATE attribute (object is only viewable after a login)
      --test-ec                 Test EC (best used with the --login or --pin option)
      --test-fork               Test forking and calling C_Initialize() in the child

~~~
