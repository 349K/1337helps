# vbutil_firmware command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:  futility vbutil_firmware <--vblock|--verify> <file> [OPTIONS]

For '--vblock <file>', required OPTIONS are:

  --keyblock <file>           Key block in .keyblock format
  --signprivate <file>        Signing private key in .vbprivk format
  --version <number>          Firmware version
  --fv <file>                 Firmware volume to sign
  --kernelkey <file>          Kernel subkey in .vbpubk format

optional OPTIONS are:
  --flags <number>            Preamble flags (defaults to 0)

For '--verify <file>', required OPTIONS are:

  --signpubkey <file>         Signing public key in .vbpubk format
  --fv <file>                 Firmware volume to verify

For '--verify <file>', optional OPTIONS are:
  --kernelkey <file>          Write the kernel subkey to this file


~~~
