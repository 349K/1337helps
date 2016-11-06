# upmpost command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

This is upMetaPost 1.9991-0.04-u1.21 (TeX Live 2016/Debian) (kpathsea version 6.2.2)

Usage: upmpost [OPTION] [&MEMNAME] [MPNAME[.mp]] [COMMANDS]
       upmpost --dvitomp DVINAME[.dvi] [MPXNAME[.mpx]]

  Run upMetaPost on MPNAME, usually creating MPNAME.NNN (and perhaps
  MPNAME.tfm), where NNN are the character numbers generated.
  Any remaining COMMANDS are processed as upMetaPost input,
  after MPNAME is read.

  With a --dvitomp argument, upMetaPost acts as DVI-to-MPX converter only.
  Call upMetaPost with --dvitomp --help for option explanations.

  -ini                      be iniupmpost, for dumping mem files
  -interaction=STRING       set interaction mode (STRING=batchmode/nonstopmode/
                            scrollmode/errorstopmode)
  -numbersystem=STRING      set number system mode (STRING=scaled/double/binary/decimal)
  -jobname=STRING           set the job name to STRING
  -kanji=STRING             set the Japanese encoding to STRING
  -progname=STRING          set program (and mem) name to STRING
  -tex=TEXPROGRAM           use TEXPROGRAM for text labels
  [-no]-file-line-error     disable/enable file:line:error style messages
  -debug                    print debugging info and leave temporary files in place
  -kpathsea-debug=NUMBER    set path searching debugging flags according to
                            the bits of NUMBER
  -mem=MEMNAME or &MEMNAME  use MEMNAME instead of program name or a %& line
  -recorder                 enable filename recorder
  -troff                    set prologues:=1 and assume TEXPROGRAM is really troff
  -s INTERNAL="STRING"      set internal INTERNAL to the string value STRING
  -s INTERNAL=NUMBER        set internal INTERNAL to the integer value NUMBER
  -help                     display this help and exit
  -version                  output version information and exit


~~~
