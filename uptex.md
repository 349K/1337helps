# uptex command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: uptex [OPTION]... [TEXNAME[.tex]] [COMMANDS]
   or: uptex [OPTION]... \FIRST-LINE
   or: uptex [OPTION]... &FMT ARGS
  Run upTeX on TEXNAME, usually creating TEXNAME.dvi.
  Any remaining COMMANDS are processed as upTeX input, after TEXNAME is read.
  If the first line of TEXNAME is %&FMT, and FMT is an existing .fmt file,
  use it.  Else use `NAME.fmt', where NAME is the program invocation name,
  most commonly `uptex'.

  Alternatively, if the first non-option argument begins with a backslash,
  interpret all non-option arguments as a line of upTeX input.

  Alternatively, if the first non-option argument begins with a &, the
  next word is taken as the FMT to read, overriding all else.  Any
  remaining arguments are processed as above.

  If no arguments or options are specified, prompt for input.

-fmt=NAME               use NAME instead of program name or %&format.
-halt-on-error          stop processing at the first error
[-no]-file-line-error   disable/enable file:line:error style messages
-ini                    be iniptex.
-interaction=STRING     set interaction mode (STRING=batchmode|nonstopmode|
                          scrollmode|errorstopmode)
-ipc                    send DVI output to a socket as well as the usual
                          output file
-ipc-start              as -ipc, and also start the server at the other end
-jobname=STRING         set the job name to STRING
-kanji=STRING           set Japanese encoding (STRING=euc|jis|sjis|utf8|uptex)
-kanji-internal=STRING  set Japanese internal encoding (STRING=euc|sjis|uptex)
-kpathsea-debug=NUMBER  set path searching debugging flags according to
                          the bits of NUMBER
[-no]-mktex=FMT         disable/enable mktexFMT generation (FMT=tex/tfm)
-mltex                  enable MLTeX extensions such as \charsubdef
-output-comment=STRING  use STRING for DVI file comment instead of date
-output-directory=DIR   use existing DIR as the directory to write files in
[-no]-parse-first-line  disable/enable parsing of first line of input file
-progname=STRING        set program (and fmt) name to STRING
-recorder               enable filename recorder
[-no]-shell-escape      disable/enable \write18{SHELL COMMAND}
-shell-restricted       enable restricted \write18
-src-specials           insert source specials into the DVI file
-src-specials=WHERE     insert source specials in certain places of
                          the DVI file. WHERE is a comma-separated value
                          list: cr display hbox math par parend vbox
-synctex=NUMBER         generate SyncTeX data for previewers if nonzero
-translate-file=TCXNAME use the TCX file TCXNAME
-help                   print this message and exit.
-version                print version information and exit.

Email bug reports to ptex-staff@ml.asciimw.jp.

~~~
