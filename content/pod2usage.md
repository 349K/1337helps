# pod2usage command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
    pod2usage   [-help] [-man] [-exit *exitval*] [-output *outfile*]
                [-verbose *level*] [-pathlist *dirlist*] [-formatter
                *module*] *file*

Options and Arguments:
    -help   Print a brief help message and exit.

    -man    Print this command's manual page and exit.

    -exit *exitval*
            The exit status value to return.

    -output *outfile*
            The output file to print to. If the special names "-" or ">&1"
            or ">&STDOUT" are used then standard output is used. If ">&2" or
            ">&STDERR" is used then standard error is used.

    -verbose *level*
            The desired level of verbosity to use:

                1 : print SYNOPSIS only
                2 : print SYNOPSIS sections and any OPTIONS/ARGUMENTS sections
                3 : print the entire manpage (similar to running pod2text)

    -pathlist *dirlist*
            Specifies one or more directories to search for the input file
            if it was not supplied with an absolute path. Each directory
            path in the given list should be separated by a ':' on Unix (';'
            on MSWin32 and DOS).

    -formatter *module*
            Which text formatter to use. Default is Pod::Text, or for very
            old Perl versions Pod::PlainText. An alternative would be e.g.
            Pod::Text::Termcap.

    *file*  The pathname of a file containing pod documentation to be output
            in usage message format (defaults to standard input).


~~~
