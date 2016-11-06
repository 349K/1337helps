# debtags command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

usage: debtags [-h] [--version] [--verbose] [--debug]
               {tag,cat,grep,check,diff,mkpatch,search,dumpavail,show,submit,tagcat,tagshow,tagsearch,update,vocfilter}
               ...

Command line interface to access and manipulate Debian Package Tags

optional arguments:
  -h, --help            show this help message and exit
  --version             show program's version number and exit
  --verbose, -v         enable verbose output
  --debug               enable debugging output (including verbose output)

subcommands:
  valid subcommands

  {tag,cat,grep,check,diff,mkpatch,search,dumpavail,show,submit,tagcat,tagshow,tagsearch,update,vocfilter}
                        additional help
    tag                 (not implemented anymore)
    cat (grep)          output the lines of the full package tag database that
                        match the given tag expression. A tag expression
                        (given as a single argument) is an arbitrarily complex
                        binary expression of tag names. For example:
                        role::program && ((use::editing || use::viewing) &&
                        !works-with::text)
    check               Check that all the tags in the given tagged collection
                        are present in the tag vocabulary. Checks the main
                        database if no file is specified
    diff (mkpatch)      Create a tag patch between the current tag database
                        and the tag collection [filename]. Standard input is
                        used if filename is not specified
    search (dumpavail)  Output the packages matching the given tag expression
    show                (deprecated) mostly the same as apt-cache show
                        <pkgnames>
    submit              (no longer supported) see
                        https://debtags.debian.org/api/patch for patch submit.
    tagcat              Output the tag vocabulary
    tagshow             Show the vocabulary information about a tag
    tagsearch           Show a summary of all tags whose data contains the
                        given strings
    update              Updates the package tag database (requires root)
                        Collect package tag data from apt cache, regenerate
                        the debtags tag database and main index. It needs to
                        be run as root
    vocfilter           Filter out the tags that are not found in the given
                        vocabulary file

~~~
