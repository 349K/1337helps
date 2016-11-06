# mf command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: mf [OPTION]... [MFNAME[.mf]] [COMMANDS]
   or: mf [OPTION]... \FIRST-LINE
   or: mf [OPTION]... &BASE ARGS
  Run Metafont on MFNAME, usually creating MFNAME.tfm and MFNAME.NNNNgf,
  where NNNN is the resolution of the specified mode (2602 by default).
  Any following COMMANDS are processed as Metafont input,
  after MFNAME is read.
  If the first line of MFNAME is %&BASE, and BASE is an existing .base file,
  use it.  Else use `NAME.base', where NAME is the program invocation name,
  most commonly `mf'.

  Alternatively, if the first non-option argument begins with a backslash,
  interpret all non-option arguments as a line of Metafont input.

  Alternatively, if the first non-option argument begins with a &, the
  next word is taken as the BASE to read, overriding all else. Any
  remaining arguments are processed as above.

  If no arguments or options are specified, prompt for input.

-base=BASENAME          use BASENAME instead of program name or a %& line
[-no]-file-line-error   disable/enable file:line:error style messages
-halt-on-error          stop processing at the first error
-ini                    be inimf, for dumping bases; this is implicitly
                          true if the program name is `inimf'
-interaction=STRING     set interaction mode (STRING=batchmode/nonstopmode/
                          scrollmode/errorstopmode)
-jobname=STRING         set the job name to STRING
-kpathsea-debug=NUMBER  set path searching debugging flags according to
                          the bits of NUMBER
[-no]-mktex=FMT         disable/enable mktexFMT generation (FMT=mf)
-output-directory=DIR   use existing DIR as the directory to write files in
[-no]-parse-first-line  disable/enable parsing of first line of input file
-progname=STRING        set program (and base) name to STRING
-recorder               enable filename recorder
-translate-file=TCXNAME use the TCX file TCXNAME
-8bit                   make all characters printable by default
-help                   display this help and exit
-version                output version information and exit

Email bug reports to tex-k@tug.org.

~~~
