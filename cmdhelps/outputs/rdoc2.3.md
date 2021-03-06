# rdoc2.3 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: rdoc2.3 [options] [names...]

  Files are parsed, and the information they contain collected, before any
  output is produced. This allows cross references between all files to be
  resolved. If a name is a directory, it is traversed. If no names are
  specified, all Ruby files in the current directory (and subdirectories) are
  processed.

  How RDoc generates output depends on the output formatter being used, and on
  the options you give.

  Options can be specified via the RDOCOPT environment variable, which
  functions similar to the RUBYOPT environment variable for ruby.

    $ export RDOCOPT="--show-hash"

  will make rdoc show hashes in method links by default.  Command-line options
  always will override those in RDOCOPT.

  Available formatters:

  darkfish - HTML generator, written by Michael Granger
  pot      - creates .pot file
  ri       - creates ri data files

  RDoc understands the following file formats:

  - C: \.(?:([CcHh])\1?|c([+xp])\2|y)\z
  - ChangeLog: (/|\\|\A)ChangeLog[^/\\]*\z
  - Markdown: \.(md|markdown)(?:\.[^.]+)?$
  - RD: \.rd(?:\.[^.]+)?$
  - Ruby: \.rbw?$
  - Simple: 
  - TomDoc:  Only in ruby files

  The following options are deprecated:

    --accessor       support discontinued
    --diagram        support discontinued
    --help-output    support discontinued
    --image-format   was an option for --diagram
    --inline-source  source code is now always inlined
    --merge          ri now always merges class information
    --one-file       support discontinued
    --op-name        support discontinued
    --opname         support discontinued
    --promiscuous    files always only document their content
    --ri-system      Ruby installers use other techniques

Parsing options:

    -e is preferred over --charset,  Specifies the output encoding.  All files
        --encoding                   read will be converted to this encoding.
                                     The default encoding is UTF-8.

        --locale=NAME                Specifies the output locale.
        --locale-data-dir=DIR        Specifies the directory where locale data live.

    -a, --all                        Synonym for --visibility=private.

    -x, --exclude=PATTERN            Do not process files or directories
                                     matching PATTERN.

    -E, --extension=NEW=OLD          Treat files ending with .new as if they
                                     ended with .old. Using '-E cgi=rb' will
                                     cause xxx.cgi to be parsed as a Ruby file.

    -U, --[no-]force-update          Forces rdoc to scan all sources even if
                                     newer than the flag file.

    -p, --pipe                       Convert RDoc on stdin to HTML

    -w, --tab-width=WIDTH            Set the width of tab characters.

        --visibility=VISIBILITY      Minimum visibility to document a method.
                                     One of 'public', 'protected' (the default),
                                     'private' or 'nodoc' (show everything)

        --markup=MARKUP              The markup format for the named files.
                                     The default is rdoc.  Valid values are:
                                     markdown, rd, rdoc, tomdoc

        --root=ROOT                  Root of the source tree documentation
                                     will be generated for.  Set this when
                                     building documentation outside the
                                     source directory.  Default is the
                                     current directory.

        --page-dir=DIR               Directory where guides, your FAQ or
                                     other pages not associated with a class
                                     live.  Set this when you don't store
                                     such files at your project root.
                                     NOTE: Do not use the same file name in
                                     the page dir and the root of your project

Common generator options:

    -O, --force-output               Forces rdoc to write the output files,
                                     even if the output directory exists
                                     and does not seem to have been created
                                     by rdoc.

    -f, --fmt, --format=FORMAT       Set the output formatter.  One of:
                                       darkfish
                                       pot
                                       ri

    -i, --include=DIRECTORIES        Set (or add to) the list of directories to
                                     be searched when satisfying :include:
                                     requests. Can be used more than once.

    -C[LEVEL],                       Prints a report on undocumented items.
        --[no-]coverage-report       Does not generate files.
        --[no-]dcov

    -o, --output, --op=DIR           Set the output directory.

    -d                               Deprecated --diagram option.
                                     Prevents firing debug mode
                                     with legacy invocation.

HTML generator options:

    -c, --charset=CHARSET            Specifies the output HTML character-set.
                                     Use --encoding instead of --charset if
                                     available.

    -A, --hyperlink-all              Generate hyperlinks for all words that
                                     correspond to known methods, even if they
                                     do not start with '#' or '::' (legacy
                                     behavior).

    -m, --main=NAME                  NAME will be the initial page displayed.

    -N, --[no-]line-numbers          Include line numbers in the source code.
                                     By default, only the number of the first
                                     line is displayed, in a leading comment.

    -H, --show-hash                  A name of the form #name in a comment is a
                                     possible hyperlink to an instance method
                                     name. When displayed, the '#' is removed
                                     unless this option is specified.

    -T, --template=NAME              Set the template used when generating
                                     output. The default depends on the
                                     formatter used.

        --template-stylesheets=FILES Set (or add to) the list of files to
                                     include with the html template.

    -t, --title=TITLE                Set TITLE as the title for HTML output.

        --copy-files=PATH            Specify a file or directory to copy static
                                     files from.
                                     If a file is given it will be copied into
                                     the output dir.  If a directory is given the
                                     entire directory will be copied.
                                     You can use this multiple times

    -W, --webcvs=URL                 Specify a URL for linking to a web frontend
                                     to CVS. If the URL contains a '%s', the
                                     name of the current file will be
                                     substituted; if the URL doesn't contain a
                                     '%s', the filename will be appended to it.

ri generator options:

    -r, --ri                         Generate output for use by `ri`. The files
                                     are stored in the '.rdoc' directory under
                                     your home directory unless overridden by a
                                     subsequent --op parameter, so no special
                                     privileges are needed.

    -R, --ri-site                    Generate output for use by `ri`. The files
                                     are stored in a site-wide directory,
                                     making them accessible to others, so
                                     special privileges are needed.

Generic options:

        --write-options              Write .rdoc_options to the current
                                     directory with the given options.  Not all
                                     options will be used.  See RDoc::Options
                                     for details.

        --[no-]dry-run               Don't write any files

    -D, --[no-]debug                 Displays lots on internal stuff.

        --[no-]ignore-invalid        Ignore invalid options and continue
                                     (default true).

    -q, --quiet                      Don't show progress as we parse.

    -V, --verbose                    Display extra progress as RDoc parses

    -v, --version                    print the version

    -h, --help                       Display this help


~~~
