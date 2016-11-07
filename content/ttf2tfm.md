# ttf2tfm command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: ttf2tfm FILE[.ttf|.ttc] [OPTION]... [FILE[.tfm]]
  Convert a TrueType font table to TeX's font metric format.

-c REAL             use REAL for height of small caps made with -V [0.8]
-e REAL             widen (extend) characters by a factor of REAL [1.0]
-E INT              select INT as the TTF encoding ID [1]
-f INT              select INT as the font index in a TTC [0]
-l                  create 1st/2nd byte ligatures in subfonts
-L LIGFILE[.sfd]    create 1st/2nd byte ligatures in subfonts using LIGFILE
-n                  use PS names of TrueType font
-N                  use only PS names and no cmap
-o FILE[.ovp]       make an OVP file for conversion to OVF and OFM
-O                  use octal for all character codes in the vpl file
-p ENCFILE[.enc]    read ENCFILE for the TTF->raw TeX mapping
-P INT              select INT as the TTF platform ID [3]
-q                  suppress informational output
-r OLDNAME NEWNAME  replace glyph name OLDNAME with NEWNAME
-R RPLFILE[.rpl]    read RPLFILE containing glyph replacement names
-s REAL             oblique (slant) characters by REAL, usually <<1 [0.0]
-t ENCFILE[.enc]    read ENCFILE for the encoding of the vpl file
-T ENCFILE[.enc]    equivalent to -p ENCFILE -t ENCFILE
-u                  output only characters from encodings, nothing extra
-v FILE[.vpl]       make a VPL file for conversion to VF
-V SCFILE[.vpl]     like -v, but synthesize smallcaps as lowercase
-w                  generate subfont enc. vectors containing glyph indices
-x                  rotate subfont glyphs by 90 degrees
-y REAL             move rotated glyphs down by a factor of REAL [0.25]
--help              print this message and exit
--version           print version number and exit

~~~
