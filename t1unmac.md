# t1unmac command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

`T1unmac' extracts a PostScript Type 1 font from a Macintosh font file. It can
read MacBinary, AppleSingle, AppleDouble, or BinHex files, or raw Macintosh
resource forks. The result is written to the standard output unless an OUTPUT
file is given.

Usage: t1unmac [OPTION]... INPUT [OUTPUT]

Options:
  -r, --raw                   Input is a raw Macintosh resource fork.
      --macbinary             Input is in MacBinary format.
      --applesingle           Input is in AppleSingle format.
      --appledouble           Input is in AppleDouble format.
      --binhex                Input is in BinHex format.
  -a, --pfa                   Output font in ASCII (PFA) format.
  -b, --pfb                   Output font in binary (PFB) format. This is
                              the default.
  -l, --block-length NUM      Set max block length for PFB output.
  -l, --line-length NUM       Set max encrypted line length for PFA output.
  -o, --output FILE           Write output to FILE.
  -h, --help                  Print this message and exit.
      --version               Print version number and warranty and exit.

Report bugs to <ekohler@gmail.com>.

~~~
