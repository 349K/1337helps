# dvihp command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dvihp [OPTIONS] [DVIFILE[.dvi]].
  Translate the given DVIFILE to Hewlett-Packard PCL by calling dvicopy
  and then $DVILJ (dvilj4 by default).
  In the absence of other options, pipe the PCL to $SPOOL (lpr by default).
  
  Options are recognized from dvips where possible:
-A    print odd pages
-B    print even pages
-d #  set debug bits to # (see documentation)
-D #  set resolution to #
-f    run as filter
-l #  don't print pages after #
-m    manual feed
-n #  print # pages
-O #,#  set/change paper offset to #,# mm
-o s  output to s instead of spooling
-p #  don't print pages before #
-Ps   pass directly to lpr
-v    verbose operation
-x #  set magnification to #

Other options are passed to the dvilj program.

Email bug reports to tex-k@tug.org.

~~~
