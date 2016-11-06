# texdoc command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: texdoc [OPTION]... NAME...
  or:  texdoc ACTION

Try to find appropriate TeX documentation for the specified NAME(s).
Alternatively, perform the given ACTION and exit.

Current settings: --view, --interact (default).

Actions:
  -h, --help            Print this help message.
  -V, --version         Print the version number.
  -f, --files           Print the list of configuration files used.
  --just-view file      Display file, given with full path (no searching).

Options:
  -w, --view            Use view mode: start a viewer. (default)
  -m, --mixed           Use mixed mode (view or list).
  -l, --list            Use list mode: show a list of results.
  -s, --showall         Use showall mode: show also "bad" results.

  -i, --interact        Use interactive menus. (default)
  -I, --nointeract      Use plain lists, no interaction required.
  -M, --machine         Machine-readable output for lists (implies -I).

  -q, --quiet           Suppress warnings and most error messages.
  -v, --verbose         Print additional information (eg, viewer command).
  -d, --debug[=list]    Activate debug output (restricted to list).

Environment: PAGER, BROWSER, PDFVIEWER, PSVIEWER, DVIVIEWER.
Files: <texmf>/texdoc/texdoc.cnf, see output of the --files option.
Report bugs to <texdoc@tug.org>.
Full manual available via `texdoc texdoc'.

~~~
