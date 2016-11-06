# pod2text command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
    pod2text [-aclostu] [--code] [--errors=*style*] [-i *indent*]
    [-q *quotes*] [--nourls] [--stderr] [-w *width*] [*input* [*output*
    ...]]

    pod2text -h

Options:
    -a, --alt
        Use an alternate output format that, among other things, uses a
        different heading style and marks "=item" entries with a colon in
        the left margin.

    --code
        Include any non-POD text from the input file in the output as well.
        Useful for viewing code documented with POD blocks with the POD
        rendered and the code left intact.

    -c, --color
        Format the output with ANSI color escape sequences. Using this
        option requires that Term::ANSIColor be installed on your system.

    -i *indent*, --indent=*indent*
        Set the number of spaces to indent regular text, and the default
        indentation for "=over" blocks. Defaults to 4 spaces if this option
        isn't given.

    -errors=*style*
        Set the error handling style. "die" says to throw an exception on
        any POD formatting error. "stderr" says to report errors on standard
        error, but not to throw an exception. "pod" says to include a POD
        ERRORS section in the resulting documentation summarizing the
        errors. "none" ignores POD errors entirely, as much as possible.

        The default is "die".

    -h, --help
        Print out usage information and exit.

    -l, --loose
        Print a blank line after a "=head1" heading. Normally, no blank line
        is printed after "=head1", although one is still printed after
        "=head2", because this is the expected formatting for manual pages;
        if you're formatting arbitrary text documents, using this option is
        recommended.

    -m *width*, --left-margin=*width*, --margin=*width*
        The width of the left margin in spaces. Defaults to 0. This is the
        margin for all text, including headings, not the amount by which
        regular text is indented; for the latter, see -i option.

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

    -o, --overstrike
        Format the output with overstrike printing. Bold text is rendered as
        character, backspace, character. Italics and file names are rendered
        as underscore, backspace, character. Many pagers, such as less, know
        how to convert this to bold or underlined text.

    -q *quotes*, --quotes=*quotes*
        Sets the quote marks used to surround C<> text to *quotes*. If
        *quotes* is a single character, it is used as both the left and
        right quote; if *quotes* is two characters, the first character is
        used as the left quote and the second as the right quoted; and if
        *quotes* is four characters, the first two are used as the left
        quote and the second two as the right quote.

        *quotes* may also be set to the special value "none", in which case
        no quote marks are added around C<> text.

    -s, --sentence
        Assume each sentence ends with two spaces and try to preserve that
        spacing. Without this option, all consecutive whitespace in
        non-verbatim paragraphs is compressed into a single space.

    --stderr
        By default, pod2text dies if any errors are detected in the POD
        input. If --stderr is given and no --errors flag is present, errors
        are sent to standard error, but pod2text does not abort. This is
        equivalent to "--errors=stderr" and is supported for backward
        compatibility.

    -t, --termcap
        Try to determine the width of the screen and the bold and underline
        sequences for the terminal from termcap, and use that information in
        formatting the output. Output will be wrapped at two columns less
        than the width of your terminal device. Using this option requires
        that your system have a termcap file somewhere where Term::Cap can
        find it and requires that your system support termios. With this
        option, the output of pod2text will contain terminal control
        sequences for your current terminal type.

    -u, --utf8
        By default, pod2text tries to use the same output encoding as its
        input encoding (to be backward-compatible with older versions). This
        option says to instead force the output encoding to UTF-8.

        Be aware that, when using this option, the input encoding of your
        POD source must be properly declared unless it is US-ASCII or
        Latin-1. POD input without an "=encoding" command will be assumed to
        be in Latin-1, and if it's actually in UTF-8, the output will be
        double-encoded. See perlpod(1) for more information on the
        "=encoding" command.

    -w, --width=*width*, -*width*
        The column at which to wrap text on the right-hand side. Defaults to
        76, unless -t is given, in which case it's two columns less than the
        width of your terminal device.


~~~
