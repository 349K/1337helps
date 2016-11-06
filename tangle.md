# tangle command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: tangle [OPTION]... WEBFILE[.web] [CHANGEFILE[.ch]]
  Tangle WEBFILE with CHANGEFILE into a Pascal program.
  Default CHANGEFILE is /dev/null;
  Pascal output goes to the basename of WEBFILE extended with `.p',
  and a string pool file, if necessary, to the same extended with `.pool'.

-length=NUMBER the first NUMBER characters of an identifier have to be
                unique (default 32)
-loose         honor the upper/lower/mixedcase and underline options when
                comparing identifiers (default)
-lowercase     make all identifiers lowercase
-mixedcase     retain the case of identifiers unchanged (default)
-strict        always smash case and remove underlines when comparing
                identifiers
-underline     do not remove underline characters from indentifiers
-uppercase     make all identifiers uppercase
-help          display this help and exit
-version       output version information and exit

Email bug reports to tex-k@tug.org.

~~~
