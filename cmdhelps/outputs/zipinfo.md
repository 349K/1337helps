# zipinfo command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


ZipInfo 3.00 of 20 April 2009, by Greg Roelofs and the Info-ZIP group.

List name, date/time, attribute, size, compression method, etc., about files
in list (excluding those in xlist) contained in the specified .zip archive(s).
"file[.zip]" may be a wildcard name containing *, ?, [] (e.g., "[a-j]*.zip").

   usage:  zipinfo [-12smlvChMtTz] file[.zip] [list...] [-x xlist...]
      or:  unzip -Z [-12smlvChMtTz] file[.zip] [list...] [-x xlist...]

main listing-format options:             -s  short Unix "ls -l" format (def.)
  -1  filenames ONLY, one per line       -m  medium Unix "ls -l" format
  -2  just filenames but allow -h/-t/-z  -l  long Unix "ls -l" format
                                         -v  verbose, multi-page format
miscellaneous options:
  -h  print header line       -t  print totals for listed files or for all
  -z  print zipfile comment   -T  print file times in sortable decimal format
  -C  be case-insensitive     -M  page output through built-in "more"
  -x  exclude filenames that follow from listing

~~~
