# gendict command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: gendict -trietype [-options] input-dictionary-file output-file
	Read in a word list and write out a string trie dictionary
options:
	-h or -? or --help  this usage text
	-V or --version     show a version message
	-c or --copyright   include a copyright notice
	-v or --verbose     turn on verbose output
	-q or --quiet       do not display warnings and progress
	-i or --icudatadir  directory for locating any needed intermediate data files,
	                    followed by path, defaults to 
	--uchars            output a UCharsTrie (mutually exclusive with -b!)
	--bytes             output a BytesTrie (mutually exclusive with -u!)
	--transform         the kind of transform to use (eg --transform offset-40A3,
	                    which specifies an offset transform with constant 0x40A3)

~~~
