# dvilualatex command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: luatex --lua=FILE [OPTION]... [TEXNAME[.tex]] [COMMANDS]
   or: luatex --lua=FILE [OPTION]... \FIRST-LINE
   or: luatex --lua=FILE [OPTION]... &FMT ARGS
  Run LuaTeX on TEXNAME, usually creating TEXNAME.pdf.
  Any remaining COMMANDS are processed as luatex input, after TEXNAME is read.

  Alternatively, if the first non-option argument begins with a backslash,
  luatex interprets all non-option arguments as an input line.

  Alternatively, if the first non-option argument begins with a &, the
  next word is taken as the FMT to read, overriding all else.  Any
  remaining arguments are processed as above.

  If no arguments or options are specified, prompt for input.

  The following regular options are understood: 

   --credits                     display credits and exit
   --debug-format                enable format debugging
   --draftmode                   switch on draft mode (generates no output PDF)
   --[no-]file-line-error        disable/enable file:line:error style messages
   --[no-]file-line-error-style  aliases of --[no-]file-line-error
   --fmt=FORMAT                  load the format file FORMAT
   --halt-on-error               stop processing at the first error
   --help                        display help and exit
   --ini                         be iniluatex, for dumping formats
   --interaction=STRING          set interaction mode (STRING=batchmode/nonstopmode/scrollmode/errorstopmode)
   --jobname=STRING              set the job name to STRING
   --kpathsea-debug=NUMBER       set path searching debugging flags according to the bits of NUMBER
   --lua=FILE                    load and execute a lua initialization script
   --[no-]mktex=FMT              disable/enable mktexFMT generation (FMT=tex/tfm)
   --nosocket                    disable the lua socket library
   --output-comment=STRING       use STRING for DVI file comment instead of date (no effect for PDF)
   --output-directory=DIR        use existing DIR as the directory to write files in
   --output-format=FORMAT        use FORMAT for job output; FORMAT is 'dvi' or 'pdf'
   --progname=STRING             set the program name to STRING
   --recorder                    enable filename recorder
   --safer                       disable easily exploitable lua commands
   --[no-]shell-escape           disable/enable system commands
   --shell-restricted            restrict system commands to a list of commands given in texmf.cnf
   --synctex=NUMBER              enable synctex
   --version                     display version and exit

Alternate behaviour models can be obtained by special switches

  --luaonly                      run a lua file, then exit
  --luaconly                     byte-compile a lua file, then exit
  --luahashchars                 the bits used by current Lua interpreter for strings hashing

See the reference manual for more information about the startup process.

Email bug reports to dev-luatex@ntg.nl.

~~~
