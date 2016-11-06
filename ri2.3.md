# ri2.3 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: ri2.3 [options] [names...]

Where name can be:

  Class | Module | Module::Class

  Class::method | Class#method | Class.method | method

  gem_name: | gem_name:README | gem_name:History

All class names may be abbreviated to their minimum unambiguous form. If a name
is ambiguous, all valid options will be listed.

A '.' matches either class or instance methods, while #method
matches only instance and ::method matches only class methods.

README and other files may be displayed by prefixing them with the gem name
they're contained in.  If the gem name is followed by a ':' all files in the
gem will be shown.  The file name extension may be omitted where it is
unambiguous.

For example:

    ri2.3 Fil
    ri2.3 File
    ri2.3 File.new
    ri2.3 zip
    ri2.3 rdoc:README

Note that shell quoting or escaping may be required for method names containing
punctuation:

    ri2.3 'Array.[]'
    ri2.3 compact\!

To see the default directories ri will search, run:

    ri2.3 --list-doc-dirs

Specifying the --system, --site, --home, --gems or --doc-dir options will
limit ri to searching only the specified directories.

ri options may be set in the 'RI' environment variable.

The ri pager can be set with the 'RI_PAGER' environment variable or the
'PAGER' environment variable.

Options:

    -i, --[no-]interactive           In interactive mode you can repeatedly
                                     look up methods with autocomplete.

    -a, --[no-]all                   Show all documentation for a class or
                                     module.

    -l, --[no-]list                  List classes ri knows about.

        --[no-]pager                 Send output directly to stdout,
                                     rather than to a pager.

    -T                               Synonym for --no-pager

    -w, --width=WIDTH                Set the width of the output.

        --server [PORT]              Run RDoc server on the given port.
                                     The default port is 8214.

    -f, --format=NAME                Uses the selected formatter. The default
                                     formatter is bs for paged output and ansi
                                     otherwise. Valid formatters are:
                                     ansi bs markdown rdoc

Data source options:

        --[no-]list-doc-dirs         List the directories from which ri will
                                     source documentation on stdout and exit.

    -d, --doc-dir=DIRNAME            List of directories from which to source
                                     documentation in addition to the standard
                                     directories.  May be repeated.

        --no-standard-docs           Do not include documentation from
                                     the Ruby standard library, site_lib,
                                     installed gems, or ~/.rdoc.
                                     Use with --doc-dir

        --[no-]system                Include documentation from Ruby's standard
                                     library.  Defaults to true.

        --[no-]site                  Include documentation from libraries
                                     installed in site_lib.
                                     Defaults to true.

        --[no-]gems                  Include documentation from RubyGems.
                                     Defaults to true.

        --[no-]home                  Include documentation stored in ~/.rdoc.
                                     Defaults to true.

Debug options:

        --[no-]profile               Run with the ruby profiler

        --dump=CACHE                 Dumps data from an ri cache or data file

~~~
