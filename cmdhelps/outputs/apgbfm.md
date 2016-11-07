# apgbfm command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~



apgbfm   APG Bloom filter management
         Copyright (c) 2001 Adel I. Mirzazhanov

apgbfm   -f filter < [-a word] | [-A dictfile] | [-n numofwords] |
                     [-c word] | [-C dictfile] | [-d dictfile] > [-s]
apgbfm   -i filter
apgbfm   [-v] [-h]

-a word        add word to filter
-A dictfile    add words from dictfile to filter
-c word        check word against filter
-C dictfile    check dictfile against filter
-n numofwords  create new empty filter
-d dictfile    create new filter and add all words from dictfile
-f filtername  use filtername as the name for filter
-q             quiet mode (do not print dots for -A and -d)
-s             create case insentive filter
-i filter      print filter information
-v             print version information
-h             print  help (this screen)

~~~
