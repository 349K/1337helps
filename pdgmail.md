# pdgmail command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: /usr/bin/pdgmail [OPTIONS]

Options:
   -f, --file       the file to use (stdin if no file given)
   -b, --bodies	    don't look for message bodies (helpful if you're getting too many false positives on the mb regex)
   -h, --help	    prints this 
   -v,--verbose	    be verbose (prints filename, other junk)
   -V,--version     prints just the version info and exits.
   
This expects to be unleashed on the result of running strings -el on a pd dump from windows process memory. Anything other than that, your mileage will certainly vary.





~~~
