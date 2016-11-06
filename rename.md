# rename command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
    rename [ -h|-m|-V ] [ -v ] [ -n ] [ -f ] [ -e|-E *perlexpr*]*|*perlexpr*
    [ *files* ]

Options:
    -v, -verbose
            Verbose: print names of files successfully renamed.

    -n, -nono
            No action: print names of files to be renamed, but don't rename.

    -f, -force
            Over write: allow existing files to be over-written.

    -h, -help
            Help: print SYNOPSIS and OPTIONS.

    -m, -man
            Manual: print manual page.

    -V, -version
            Version: show version number.

    -e      Expression: code to act on files name.

            May be repeated to build up code (like "perl -e"). If no -e, the
            first argument is used as code.

    -E      Statement: code to act on files name, as -e but terminated by
            ';'.


~~~
