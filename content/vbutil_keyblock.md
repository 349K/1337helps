# vbutil_keyblock command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:  futility vbutil_keyblock <--pack|--unpack> <file> [OPTIONS]

For '--pack <file>', required OPTIONS are:
  --datapubkey <file>         Data public key in .vbpubk format

Optional OPTIONS are:
  --signprivate <file>        Signing private key in .vbprivk format.
OR
  --signprivate_pem <file>
  --pem_algorithm <algo>
        Signing private key in .pem format and algorithm id.
(If one of the above arguments is not specified, the keyblock will
not be signed.)

  --flags <number>            Specifies allowed use conditions.
  --externalsigner "cmd"        Use an external program cmd to calculate the signatures.

For '--unpack <file>', optional OPTIONS are:
  --signpubkey <file>        Signing public key in .vbpubk format. This is required to
                                verify a signed keyblock.
  --datapubkey <file>        Write the data public key to this file.


~~~
