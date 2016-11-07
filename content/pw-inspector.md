# pw-inspector command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

PW-Inspector v0.2 (c) 2005 by van Hauser / THC vh@thc.org [http://www.thc.org]

Syntax: pw-inspector [-i FILE] [-o FILE] [-m MINLEN] [-M MAXLEN] [-c MINSETS] -l -u -n -p -s

Options:
  -i FILE    file to read passwords from (default: stdin)
  -o FILE    file to write valid passwords to (default: stdout)
  -m MINLEN  minimum length of a valid password
  -M MAXLEN  maximum length of a valid password
  -c MINSETS the minimum number of sets required (default: all given)
Sets:
  -l         lowcase characters (a,b,c,d, etc.)
  -u         upcase characters (A,B,C,D, etc.)
  -n         numbers (1,2,3,4, etc.)
  -p         printable characters (which are not -l/-n/-p, e.g. $,!,/,(,*, etc.)
  -s         special characters - all others not withint the sets above

PW-Inspector reads passwords in and prints those which meet the requirements.
The return code is the number of valid passwords found, 0 if none was found.
Use for security: check passwords, if 0 is returned, reject password choice.
Use for hacking: trim your dictionary file to the pw requirements of the target.
Usage only allowed for legal purposes.

~~~
