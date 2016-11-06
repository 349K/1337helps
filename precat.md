# precat command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

prezip, a prefix delta compressor. Version 0.1.1, 2004-11-06

  usage /usr/bin/precat [-dzhLV] [-cfksSq] [file ...]

   -h --help        display help
   -d --decompress  force decompression
   -z --compress    dorce compression
   -L --license     display software license
   -V --version     display version

   -c --stdout      decompress to standard output
   -f --force       force
   -k --keep        keep input files
   -s --sort        sort and remove duplicates before compressing
   -S --nocwl       do not rename .wl suffix to .cwl (use .wl.pz instead)
   -q --quiet       suppress all warnings

  If invoked as "prezip" the default action is to compress.
             as "preunzip" the default action is to decompress.
             as "precat" the default action is to decompress to stdout.

  If no file names are given then prezip will compress or decompress
  from the standard input to the standard output.  Short flags can be
  combined so that "-c -s" is the same as "-cs".

  Prezip is _not_ a general purpose compressor.  It should only be
  used on sorted word lists or other similar text files.  It will
  likely _increase_ the size of binary data.


~~~
