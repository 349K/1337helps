# zipnote command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Copyright (c) 1990-2008 Info-ZIP - Type 'zipnote "-L"' for software license.

ZipNote 3.0 (July 5th 2008)
Usage:  zipnote [-w] [-q] [-b path] zipfile
  the default action is to write the comments in zipfile to stdout
  -w   write the zipfile comments from stdin
  -b   use "path" for the temporary zip file
  -q   quieter operation, suppress some informational messages
  -h   show this help    -v   show version info    -L   show software license

Example:
     zipnote foo.zip > foo.tmp
     ed foo.tmp
     ... then you edit the comments, save, and exit ...
     zipnote -w foo.zip < foo.tmp

  "@ name" can be followed by an "@=newname" line to change the name

~~~
