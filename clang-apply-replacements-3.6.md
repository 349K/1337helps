# clang-apply-replacements-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

USAGE: clang-apply-replacements-3.6 [options] <Search Root Directory>

OPTIONS:

Formatting Options:

  -format                   - Enable formatting of code changed by applying replacements.
                              Use -style to choose formatting style.
  -style=<string>           - Coding style, currently supports:
                                LLVM, Google, Chromium, Mozilla, WebKit.
                              Use -style=file to load style configuration from
                              .clang-format file located in one of the parent
                              directories of the source file (or current
                              directory for stdin).
                              Use -style="{key: value, ...}" to set specific
                              parameters, e.g.:
                                -style="{BasedOnStyle: llvm, IndentWidth: 8}"
  -style-config=<string>    - Path to a directory containing a .clang-format file
                              describing a formatting style to use for formatting
                              code when -style=file.

General options:

  -help                     - Display available options (-help-hidden for more)
  -help-list                - Display list of available options (-help-list-hidden for more)
  -remove-change-desc-files - Remove the change description files regardless of successful
                              merging/replacing.
  -version                  - Display the version of this program

~~~
