# cweave command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: cweave [OPTIONS] WEBFILE[.w] [{CHANGEFILE[.ch]|-} [OUTFILE[.tex]]]
  Weave WEBFILE with CHANGEFILE into a TeX document.
  Default CHANGEFILE is /dev/null;
  TeX output goes to the basename of WEBFILE extended with `.tex'
  unless otherwise specified by OUTFILE; in this case, '-' specifies
  a null CHANGEFILE.

-b          suppress banner line on terminal
-f          do not force a newline after every C statement in output
-h          suppress success message on completion
-p          suppress progress report messages
-x          omit indices and table of contents
+e          enclose C material in \PB{...}
+s          print usage statistics
--help      display this help and exit
--version   output version information and exit

Email bug reports to tex-k@tug.org.

~~~
