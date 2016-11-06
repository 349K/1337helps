# vbutil_kernel command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:  futility vbutil_kernel --pack <file> [PARAMETERS]

  Required parameters:
    --keyblock <file>         Key block in .keyblock format
    --signprivate <file>      Private key to sign kernel data,
                                in .vbprivk format
    --version <number>        Kernel version
    --vmlinuz <file>          Linux kernel bzImage file
    --bootloader <file>       Bootloader stub
    --config <file>           Command line file
    --arch <arch>             Cpu architecture (default x86)

  Optional:
    --kloadaddr <address>     Assign kernel body load address
    --pad <number>            Verification padding size in bytes
    --vblockonly              Emit just the verification blob
    --flags NUM               Flags to be passed in the header

OR

Usage:  futility vbutil_kernel --repack <file> [PARAMETERS]

  Required parameters:
    --signprivate <file>      Private key to sign kernel data,
                                in .vbprivk format
    --oldblob <file>          Previously packed kernel blob
                                (including verfication blob)

  Optional:
    --keyblock <file>         Key block in .keyblock format
    --config <file>           New command line file
    --version <number>        Kernel version
    --kloadaddr <address>     Assign kernel body load address
    --pad <number>            Verification blob size in bytes
    --vblockonly              Emit just the verification blob

OR

Usage:  futility vbutil_kernel --verify <file> [PARAMETERS]

  Optional:
    --signpubkey <file>       Public key to verify kernel keyblock,
                                in .vbpubk format
    --verbose                 Print a more detailed report
    --keyblock <file>         Outputs the verified key block,
                                in .keyblock format
    --pad <number>            Verification padding size in bytes
    --minversion <number>     Minimum combined kernel key version

OR

Usage:  futility vbutil_kernel --get-vmlinuz <file> [PARAMETERS]

  Required parameters:
    --vmlinuz-out <file>      vmlinuz image output file


~~~
