# pod2man command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
    pod2man [--center=*string*] [--date=*string*] [--errors=*style*]
    [--fixed=*font*] [--fixedbold=*font*] [--fixeditalic=*font*]
    [--fixedbolditalic=*font*] [--name=*name*] [--nourls] [--official]
    [--quotes=*quotes*] [--release[=*version*]] [--section=*manext*]
    [--stderr] [--utf8] [--verbose] [*input* [*output*] ...]

    pod2man --help

Options:
    -c *string*, --center=*string*
        Sets the centered page header to *string*. The default is "User
        Contributed Perl Documentation", but also see --official below.

    -d *string*, --date=*string*
        Set the left-hand footer string to this value. By default, the
        modification date of the input file will be used, or the current
        date if input comes from "STDIN", and will be based on UTC (so that
        the output will be reproducible regardless of local time zone).

    -errors=*style*
        Set the error handling style. "die" says to throw an exception on
        any POD formatting error. "stderr" says to report errors on standard
        error, but not to throw an exception. "pod" says to include a POD
        ERRORS section in the resulting documentation summarizing the
        errors. "none" ignores POD errors entirely, as much as possible.

        The default is "die".

    --fixed=*font*
        The fixed-width font to use for verbatim text and code. Defaults to
        "CW". Some systems may want "CR" instead. Only matters for troff(1)
        output.

    --fixedbold=*font*
        Bold version of the fixed-width font. Defaults to "CB". Only matters
        for troff(1) output.

    --fixeditalic=*font*
        Italic version of the fixed-width font (actually, something of a
        misnomer, since most fixed-width fonts only have an oblique version,
        not an italic version). Defaults to "CI". Only matters for troff(1)
        output.

    --fixedbolditalic=*font*
        Bold italic (probably actually oblique) version of the fixed-width
        font. Pod::Man doesn't assume you have this, and defaults to "CB".
        Some systems (such as Solaris) have this font available as "CX".
        Only matters for troff(1) output.

    -h, --help
        Print out usage information.

    -l, --lax
        No longer used. pod2man used to check its input for validity as a
        manual page, but this should now be done by podchecker(1) instead.
        Accepted for backward compatibility; this option no longer does
        anything.

    -n *name*, --name=*name*
        Set the name of the manual page to *name*. Without this option, the
        manual name is set to the uppercased base name of the file being
        converted unless the manual section is 3, in which case the path is
        parsed to see if it is a Perl module path. If it is, a path like
        ".../lib/Pod/Man.pm" is converted into a name like "Pod::Man". This
        option, if given, overrides any automatic determination of the name.

        Note that this option is probably not useful when converting
        multiple POD files at once. The convention for Unix man pages for
        commands is for the man page title to be in all-uppercase even if
        the command isn't.

        When converting POD source from standard input, this option is
        required, since there's otherwise no way to know what to use as the
        name of the manual page.

    --nourls
        Normally, L<> formatting codes with a URL but anchor text are
        formatted to show both the anchor text and the URL. In other words:

            L<foo|http://example.com/>

        is formatted as:

            foo <http://example.com/>

        This flag, if given, suppresses the URL when anchor text is given,
        so this example would be formatted as just "foo". This can produce
        less cluttered output in cases where the URLs are not particularly
        important.

    -o, --official
        Set the default header to indicate that this page is part of the
        standard Perl release, if --center is not also given.

    -q *quotes*, --quotes=*quotes*
        Sets the quote marks used to surround C<> text to *quotes*. If
        *quotes* is a single character, it is used as both the left and
        right quote; if *quotes* is two characters, the first character is
        used as the left quote and the second as the right quoted; and if
        *quotes* is four characters, the first two are used as the left
        quote and the second two as the right quote.

        *quotes* may also be set to the special value "none", in which case
        no quote marks are added around C<> text (but the font is still
        changed for troff output).

    -r, --release
        Set the centered footer. By default, this is the version of Perl you
        run pod2man under. Note that some system an macro sets assume that
        the centered footer will be a modification date and will prepend
        something like "Last modified: "; if this is the case, you may want
        to set --release to the last modified date and --date to the version
        number.

    -s, --section
        Set the section for the ".TH" macro. The standard section numbering
        convention is to use 1 for user commands, 2 for system calls, 3 for
        functions, 4 for devices, 5 for file formats, 6 for games, 7 for
        miscellaneous information, and 8 for administrator commands. There
        is a lot of variation here, however; some systems (like Solaris) use
        4 for file formats, 5 for miscellaneous information, and 7 for
        devices. Still others use 1m instead of 8, or some mix of both.
        About the only section numbers that are reliably consistent are 1,
        2, and 3.

        By default, section 1 will be used unless the file ends in ".pm", in
        which case section 3 will be selected.

    --stderr
        By default, pod2man dies if any errors are detected in the POD
        input. If --stderr is given and no --errors flag is present, errors
        are sent to standard error, but pod2man does not abort. This is
        equivalent to "--errors=stderr" and is supported for backward
        compatibility.

    -u, --utf8
        By default, pod2man produces the most conservative possible *roff
        output to try to ensure that it will work with as many different
        *roff implementations as possible. Many *roff implementations cannot
        handle non-ASCII characters, so this means all non-ASCII characters
        are converted either to a *roff escape sequence that tries to create
        a properly accented character (at least for troff output) or to "X".

        This option says to instead output literal UTF-8 characters. If your
        *roff implementation can handle it, this is the best output format
        to use and avoids corruption of documents containing non-ASCII
        characters. However, be warned that *roff source with literal UTF-8
        characters is not supported by many implementations and may even
        result in segfaults and other bad behavior.

        Be aware that, when using this option, the input encoding of your
        POD source must be properly declared unless it is US-ASCII or
        Latin-1. POD input without an "=encoding" command will be assumed to
        be in Latin-1, and if it's actually in UTF-8, the output will be
        double-encoded. See perlpod(1) for more information on the
        "=encoding" command.

    -v, --verbose
        Print out the name of each output file as it is being generated.


~~~
