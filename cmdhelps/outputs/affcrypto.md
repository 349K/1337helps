# affcrypto command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

affcrypto version 3.7.10
usage: affcrypto [options] filename.aff [filename2.aff ... ]
   prints if each file is encrypted or not.
options:
    -x      --- output in XML
    -j      --- Just print the number of encrypted segments
    -J      --- Just print the number of unencrypted segments

Data conversion options:
    -e      --- encrypt the unencrypted non-signature segments
    -d      --- decrypt the encrypted non-signature segments
    -r      --- change passphrase (take old and new from stdin)
    -O old  --- specify old passphrase
    -N new  --- specify new passphrase
    -K mykey.key  -- specifies a private keyfile for unsealing (may not be repeated)
    -C mycert.crt -- specifies a certificate file for sealing (may be repeated)
    -S      --- add symmetric encryptiong (passphrase) to AFFILE encrypted with public key
                    (requires a private key and a specified passphrase).
    -A      --- add asymmetric encryption to a AFFILE encrypted with a passphrase
                    (requires a certificate file spcified with the -C option

Password Cracking Options:
    -p passphrase --- checks to see if passphrase is the passphrase of the file
                exit code is 0 if it is, -1 if it is not
    -k      --- attempt to crack passwords by reading a list of passwords from ~/.affpassphrase
    -f file --- Crack passwords but read them from file.

Debugging:
    -V      --- Just print the version number and exit.
    -D      --- debug; print out each key as it is tried
    -l      --- List the installed hash and encryption algorithms 
Note: This program ignores the environment variables:
AFFLIB_PASSPHRASE
AFFLIB_PASSPHRASE_FILE
AFFLIB_PASSPHRASE_FD
AFFLIB_DECRYPTING_PRIVATE_KEYFILE

~~~
