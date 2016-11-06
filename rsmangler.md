# rsmangler command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

rsmangler v 1.4 Robin Wood (robin@digininja.org) <www.randomstorm.com>

To pass the initial words in on standard in do:

cat wordlist.txt | ./rsmangler.rb --file - > new_wordlist.rb

All options are ON by default, these parameters turn them OFF

Usage: rsmangler.rb [OPTION]
	--help, -h: show help
	--file, -f: the input file, use - for STDIN
	--max, -x: maximum word length
	--min, -m: minimum word length
	--perms, -p: permutate all the words
	--double, -d: double each word
	--reverse, -r: reverser the word
	--leet, -t: l33t speak the word
	--full-leet, -T: all posibilities l33t
	--capital, -c: capitalise the word
	--upper, -u: uppercase the word
	--lower, -l: lowercase the word
	--swap, -s: swap the case of the word
	--ed, -e: add ed to the end of the word
	--ing, -i: add ing to the end of the word
	--punctuation: add common punctuation to the end of the word
	--years, -y: add all years from 1990 to current year to start and end
	--acronym, -a: create an acronym based on all the words entered in order and add to word list
	--common, -C: add the following words to start and end: admin, sys, pw, pwd
	--pna: add 01 - 09 to the end of the word
	--pnb: add 01 - 09 to the beginning of the word
	--na: add 1 - 123 to the end of the word
	--nb: add 1 - 123 to the beginning of the word
	--force - don't check ooutput size
	--space - add spaces between words


~~~
