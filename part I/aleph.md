# aleph command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: aleph [OPTION]... [TEXNAME[.tex]] [COMMANDS]
   or: aleph [OPTION]... \FIRST-LINE
   or: aleph [OPTION]... &FMT ARGS
  Run Aleph on TEXNAME, usually creating TEXNAME.dvi.
  Any remaining COMMANDS are processed as Aleph input, after TEXNAME is read.
  If the first line of TEXNAME is %&FMT, and FMT is an existing .fmt file,
  use it.  Else use `NAME.fmt', where NAME is the program invocation name,
  most commonly `aleph'.

  Alternatively, if the first non-option argument begins with a backslash,
  interpret all non-option arguments as a line of Aleph input.

  Alternatively, if the first non-option argument begins with a &, the
  next word is taken as the FMT to read, overriding all else.  Any
  remaining arguments are processed as above.

  If no arguments or options are specified, prompt for input.

-etex                   enable e-TeX extensions
[-no]-file-line-error   disable/enable file:line:error style messages
-fmt=FMTNAME            use FMTNAME instead of program name or a %& line
-halt-on-error          stop processing at the first error
-ini                    be inialeph, for dumping formats; this is implicitly
                          true if the program name is `inialeph'
-interaction=STRING     set interaction mode (STRING=batchmode/nonstopmode/
                          scrollmode/errorstopmode)
-ipc                    send DVI output to a socket as well as the usual
                          output file
-ipc-start              as -ipc, and also start the server at the other end
-jobname=STRING         set the job name to STRING
-kpathsea-debug=NUMBER  set path searching debugging flags according to the
                          bits of NUMBER
[-no]-mktex=FMT         disable/enable mktexFMT generation (FMT=tex/tfm)
-output-comment=STRING  use STRING for DVI file comment instead of date
-output-directory=DIR   use existing DIR as the directory to write files in
[-no]-parse-first-line  disable/enable parsing of first line of input file
-progname=STRING        set program (and fmt) name to STRING
-recorder               enable filename recorder (always on)
[-no]-shell-escape      disable/enable \write18{SHELL COMMAND}
-shell-restricted       enable restricted \write18
-src-specials           insert source specials into the DVI file
-src-specials=WHERE     insert source specials in certain places of
                          the DVI file. WHERE is a comma-separated value
                          list: cr display hbox math par parend vbox
-help                   display this help and exit
-version                output version information and exit

Email bug reports to tex-k@tug.org.

~~~
