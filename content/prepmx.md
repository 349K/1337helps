# prepmx command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


==> This is M-Tx 0.62 (Music from TeXt) <08 February 2016>
Usage: prepmx [-bcfnhimtuvwDH0123456789] MTXFILE [TEXDIR] [STYLEFILE]

MTXFILE: name of .mtx file without its extension
TEXDIR: directory where the TeX file made by PMX goes, default is ./
STYLEFILE: name of a file containing style definitions.  Default is
  mtxstyle.txt.  This feature is now deprecated; use Include: STYLEFILE
  in the preamble of the .mtx file instead.
Options:  (can also be entered separately: -b -c ...)
  -b: disable unbeamVocal
  -c: disable doChords
  -f: enable solfaNoteNames
  -h: display this message and quit
  -i: enable ignoreErrors
  -m: disable doLyrics
  -n: enable instrumentNames
  -t: disable doUptext
  -u: disable uptextOnRests
  -v: enable beVerbose
  -w: enable pedanticWarnings
  -D: enable debugMode
  -0123456789: select Case
  -H: print enabled status of all options
All the above, and some other, options can be enabled or disabled
  in the preamble.  What you do there overrides what you do here.

~~~
