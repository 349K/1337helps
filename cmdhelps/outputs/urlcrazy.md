# urlcrazy command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

URLCrazy version 0.5
by Andrew Horton (urbanadventurer)
http://www.morningstarsecurity.com/research/urlcrazy

Generate and test domain typos and variations to detect and perform typo squatting, URL hijacking,
phishing, and corporate espionage.

Supports the following domain variations:
Character omission, character repeat, adjacent character swap, adjacent character replacement, double 
character replacement, adjacent character insertion, missing dot, strip dashes, singular or pluralise,
common misspellings, vowel swaps, homophones, bit flipping (cosmic rays), homoglyphs, wrong top level 
domain, and wrong second level domain.

Usage: /usr/bin/urlcrazy [options] domain

Options
 -k, --keyboard=LAYOUT	Options are: qwerty, azerty, qwertz, dvorak (default: qwerty)
 -p, --popularity	Check domain popularity with Google
 -r, --no-resolve	Do not resolve DNS
 -i, --show-invalid	Show invalid domain names
 -f, --format=TYPE	Human readable or CSV (default: human readable)
 -o, --output=FILE	Output file
 -h, --help		This help
 -v, --version   	Print version information. This version is 0.5


~~~
