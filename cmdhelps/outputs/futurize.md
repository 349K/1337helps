# futurize command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: futurize [options] file|dir ...

Options:
  -h, --help            show this help message and exit
  -V, --version         Report the version number of futurize
  -a, --all-imports     Add all __future__ and future imports to each module
  -1, --stage1          Modernize Python 2 code only; no compatibility with
                        Python 3 (or dependency on ``future``)
  -2, --stage2          Take modernized (stage1) code and add a dependency on
                        ``future`` to provide Py3 compatibility.
  -0, --both-stages     Apply both stages 1 and 2
  -u, --unicode-literals
                        Add ``from __future__ import unicode_literals`` to
                        implicitly convert all unadorned string literals ''
                        into unicode strings
  -f FIX, --fix=FIX     Each FIX specifies a transformation; default: all.
                        Either use '-f division -f metaclass' etc. or use the
                        fully-qualified module name: '-f
                        lib2to3.fixes.fix_types -f
                        libfuturize.fixes.fix_unicode_keep_u'
  -j PROCESSES, --processes=PROCESSES
                        Run 2to3 concurrently
  -x NOFIX, --nofix=NOFIX
                        Prevent a fixer from being run.
  -l, --list-fixes      List available transformations
  -p, --print-function  Modify the grammar so that print() is a function
  -v, --verbose         More verbose logging
  --no-diffs            Don't show diffs of the refactoring
  -w, --write           Write back modified files
  -n, --nobackups       Don't write backups for modified files.
  -o OUTPUT_DIR, --output-dir=OUTPUT_DIR
                        Put output files in this directory instead of
                        overwriting the input files.  Requires -n. For Python
                        >= 2.7 only.
  -W, --write-unchanged-files
                        Also write files even if no changes were required
                        (useful with --output-dir); implies -w.
  --add-suffix=ADD_SUFFIX
                        Append this string to all output filenames. Requires
                        -n if non-empty. For Python >= 2.7 only.ex: --add-
                        suffix='3' will generate .py3 files.

~~~
