# bmpblk_utility command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~



To create a new BMPBLOCK file using config from YAML file:

  bmpblk_utility [-z NUM] -c YAML BMPBLOCK

    -z NUM  = compression algorithm to use
              0 = none
              1 = EFIv1
              2 = LZMA1

To display the contents of a BMPBLOCK:

  bmpblk_utility [-y] BMPBLOCK

    -y  = display as yaml

To unpack a BMPBLOCK file:

  bmpblk_utility -x [-d DIR] [-f] BMPBLOCK

    -d DIR  = directory to use (default '.')
    -f      = force overwriting existing files


~~~
