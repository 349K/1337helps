# rulegen command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: rulegen [options] passwords.txt

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -b rockyou, --basename=rockyou
                        Output base name. The following files will be
                        generated: basename.words, basename.rules and
                        basename.stats
  -w wiki.dict, --wordlist=wiki.dict
                        Use a custom wordlist for rule analysis.
  -q, --quiet           Don't show headers.
  --threads=THREADS     Parallel threads to use for processing.

  Fine tune source word generation::
    --maxworddist=10    Maximum word edit distance (Levenshtein)
    --maxwords=5        Maximum number of source word candidates to consider
    --morewords         Consider suboptimal source word candidates
    --simplewords       Generate simple source words for given passwords

  Fine tune rule generation::
    --maxrulelen=10     Maximum number of operations in a single rule
    --maxrules=5        Maximum number of rules to consider
    --morerules         Generate suboptimal rules
    --simplerules       Generate simple rules insert,delete,replace
    --bruterules        Bruteforce reversal and rotation rules (slow)

  Fine tune spell checker engine::
    --providers=aspell,myspell
                        Comma-separated list of provider engines

  Debuggin options::
    -v, --verbose       Show verbose information.
    -d, --debug         Debug rules.
    --password          Process the last argument as a password not a file.
    --word=Password     Use a custom word for rule analysis
    --hashcat           Test generated rules with hashcat-cli

~~~
