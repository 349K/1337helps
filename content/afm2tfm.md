# afm2tfm command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: afm2tfm FILE[.afm] [OPTION]... [FILE[.tfm]]
  Convert an Adobe font metric file to TeX font metric format.

-a                  omit heuristic adjustment of heights for accents
-c REAL             use REAL for height of small caps made with -V [0.8]
-e REAL             widen (extend) characters by a factor of REAL
-O                  use octal for all character codes in the vpl file
-p ENCFILE          read/download ENCFILE for the PostScript encoding
-s REAL             oblique (slant) characters by REAL, generally <<1
-t ENCFILE          read ENCFILE for the encoding of the vpl file
-T ENCFILE          equivalent to -p ENCFILE -t ENCFILE
-u                  output only characters from encodings, nothing extra
-v FILE[.vpl]       make a VPL file for conversion to VF
-V SCFILE[.vpl]     like -v, but synthesize smallcaps as lowercase
--help              print this message and exit.
--version           print version number and exit.

Email bug reports to tex-k@tug.org.

~~~
