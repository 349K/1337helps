# t1mac command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

`T1mac' translates a PostScript Type 1 font from PFA or PFB format into
Macintosh Type 1 format. The result can be written in MacBinary II format (the
default), AppleSingle format, AppleDouble format, or BinHex format, or as a
raw resource fork. It is sent to the standard output unless an OUTPUT file is
given.

Usage: t1mac [OPTION]... [INPUT [OUTPUT]]

Options:
  -r, --raw                   Output is a raw Macintosh resource fork.
      --macbinary             Output is in MacBinary format (default).
      --applesingle           Output is in AppleSingle format.
      --appledouble           Output is in AppleDouble format.
      --binhex                Output is in BinHex format.
  -n, --filename NAME         Macintosh font filename will be NAME.
  -o, --output FILE           Write output to FILE.
  -h, --help                  Print this message and exit.
      --version               Print version number and warranty and exit.

Report bugs to <ekohler@gmail.com>.

~~~
