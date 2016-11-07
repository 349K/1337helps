# mimetype command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
    mimetype [options] [-] files

Options:
    -a, --all
        Show output of all rules that match the file.

        TODO: this method now just returns one match for each method (globs,
        magic, etc.).

    -b, --brief
        Do not prepend filenames to output lines (brief mode).

    --database=*mimedir*:*mimedir*:...
        Force the program to look in these directories for the shared
        mime-info database. The directories specified by the basedir
        specification are ignored.

    -d, --describe
        Print file descriptions instead of mime types, this is the default
        when using "--file-compat".

    -D, --debug
        Print debug information about how the mimetype was determined.

    -f *namefile*, --namefile=*namefile*
        Read the names of the files to be examined from the file 'namefile'
        (one per line) before the argument list.

    --file-compat
        Make mimetype behave a little more file(1) compatible. This is
        turned on automatically when you call mimetype by a link called
        'file'.

        A single '-' won't be considered a separator between options and
        filenames anymore, but becomes identical to "--stdin". ( You can
        still use '--' as separator, but that is not backward compatible
        with the original file command. ) Also the default becomes to print
        descriptions instead of mimetypes.

    -F *string*, --separator=*string*
        Use string as custom separator between the file name and its
        mimetype or description, defaults to ':' .

    -h, --help
    -u, --usage
        Print a help message and exits.

    -i, --mimetype
        Use mime types, opposite to "--describe", this is the default when
        _not_ using "--file-compat".

    -L, --dereference
        Follow symbolic links.

    -l *code*, --language=*code*
        The language attribute specifies a two letter language code, this
        makes descriptions being outputted in the specified language.

    -M, --magic-only
        Do not check for extensions, globs or inode type, only look at the
        content of the file. This is particularly useful if for some reason
        you don't trust the name or the extension a file has.

    -N, --noalign
        Do not align output fields.

    --output-format
        If you want an alternative output format, you can specify a format
        string containing the following escapes:

                %f for the filename
                %d description
                %m mime type

        Alignment is not available when using this, you need to post-process
        the output to do that.

    --stdin
        Determine type of content from STDIN, less powerful then normal file
        checking because it only uses magic typing. This will happen also if
        the STDIN filehandle is a pipe.

        To use this option IO::Scalar needs to be installed.

    -v, --version
        Print the version of the program and exit.


~~~
