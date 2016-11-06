# mimeopen command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
    mimeopen [options] [-] files

Options:
    -a, --ask
        Do not execute the default application but ask which application to
        run. This does not change the default application.

    -d, --ask-default
        Let the user choose a new default program for given files.

    -n, --no-ask
        Don't ask the user which program to use. Choose the default program
        or the first program known to handle the file mimetype. This does
        not set the default application.

    -M, --magic-only
        Do not check for extensions, globs or inode type, only look at the
        content of the file. This is particularly useful if for some reason
        you don't trust the name or the extension a file has.

    --database=*mimedir*:*mimedir*:...
        Force the program to look in these directories for the shared
        mime-info database. The directories specified by the basedir
        specification are ignored.

    -D, --debug
        Print debug information about how the mimetype was determined.

    -h, --help
    -u, --usage
        Print a help message and exits.

    -v, --version
        Print the version of the program and exit.


~~~
