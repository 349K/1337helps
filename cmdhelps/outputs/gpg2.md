# gpg2 command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


gpg (GnuPG) 2.1.11
libgcrypt 1.7.3-beta
Copyright (C) 2016 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

Home: ~/.gnupg
Supported algorithms:
Pubkey: RSA, ELG, DSA, ECDH, ECDSA, EDDSA
Cipher: IDEA, 3DES, CAST5, BLOWFISH, AES, AES192, AES256, TWOFISH,
        CAMELLIA128, CAMELLIA192, CAMELLIA256
Hash: SHA1, RIPEMD160, SHA256, SHA384, SHA512, SHA224
Compression: Uncompressed, ZIP, ZLIB, BZIP2

Syntax: gpg [options] [files]
Sign, check, encrypt or decrypt
Default operation depends on the input data

Commands:
 
 -s, --sign                 make a signature
     --clearsign            make a clear text signature
 -b, --detach-sign          make a detached signature
 -e, --encrypt              encrypt data
 -c, --symmetric            encryption only with symmetric cipher
 -d, --decrypt              decrypt data (default)
     --verify               verify a signature
 -k, --list-keys            list keys
     --list-sigs            list keys and signatures
     --check-sigs           list and check key signatures
     --fingerprint          list keys and fingerprints
 -K, --list-secret-keys     list secret keys
     --gen-key              generate a new key pair
     --quick-gen-key        quickly generate a new key pair
     --quick-adduid         quickly add a new user-id
     --full-gen-key         full featured key pair generation
     --gen-revoke           generate a revocation certificate
     --delete-keys          remove keys from the public keyring
     --delete-secret-keys   remove keys from the secret keyring
     --quick-sign-key       quickly sign a key
     --quick-lsign-key      quickly sign a key locally
     --sign-key             sign a key
     --lsign-key            sign a key locally
     --edit-key             sign or edit a key
     --passwd               change a passphrase
     --export               export keys
     --send-keys            export keys to a key server
     --recv-keys            import keys from a key server
     --search-keys          search for keys on a key server
     --refresh-keys         update all keys from a keyserver
     --import               import/merge keys
     --card-status          print the card status
     --card-edit            change data on a card
     --change-pin           change a card's PIN
     --update-trustdb       update the trust database
     --print-md             print message digests
     --server               run in server mode
     --tofu-policy VALUE    set the TOFU policy for a key (good, unknown, bad, ask, auto)

Options:
 
 -a, --armor                create ascii armored output
 -r, --recipient USER-ID    encrypt for USER-ID
 -u, --local-user USER-ID   use USER-ID to sign or decrypt
 -z N                       set compress level to N (0 disables)
     --textmode             use canonical text mode
 -o, --output FILE          write output to FILE
 -v, --verbose              verbose
 -n, --dry-run              do not make any changes
 -i, --interactive          prompt before overwriting
     --openpgp              use strict OpenPGP behavior

(See the man page for a complete listing of all commands and options)

Examples:

 -se -r Bob [file]          sign and encrypt for user Bob
 --clearsign [file]         make a clear text signature
 --detach-sign [file]       make a detached signature
 --list-keys [names]        show keys
 --fingerprint [names]      show fingerprints

Please report bugs to <http://bugs.gnupg.org>.

~~~
