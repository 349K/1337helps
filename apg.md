# apg command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~



apg   Automated Password Generator
        Copyright (c) Adel I. Mirzazhanov

apg   [-a algorithm] [-r file] 
      [-M mode] [-E char_string] [-n num_of_pass] [-m min_pass_len]
      [-x max_pass_len] [-c cl_seed] [-d] [-s] [-h] [-y] [-q]

-M mode         new style password modes
-E char_string  exclude characters from password generation process
-r file         apply dictionary check against file
-b filter_file  apply bloom filter check against filter_file
                (filter_file should be created with apgbfm(1) utility)
-p substr_len   paranoid modifier for bloom filter check
-a algorithm    choose algorithm
                 1 - random password generation according to
                     password modes
                 0 - pronounceable password generation
-n num_of_pass  generate num_of_pass passwords
-m min_pass_len minimum password length
-x max_pass_len maximum password length
-s              ask user for a random seed for password
                generation
-c cl_seed      use cl_seed as a random seed for password
-d              do NOT use any delimiters between generated passwords
-l              spell generated password
-t              print pronunciation for generated pronounceable password
-y              print crypted passwords
-q              quiet mode (do not print warnings)
-h              print this help screen
-v              print version information

~~~
