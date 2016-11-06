# html2markdown.py2 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: html2markdown.py2 [(filename|url) [encoding]]

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  --pad-tables          pad the cells to equal column width in tables
  --no-wrap-links       wrap links during conversion
  --ignore-emphasis     don't include any formatting for emphasis
  --reference-links     use reference style links instead of inline links
  --ignore-links        don't include any formatting for links
  --protect-links       protect links from line breaks surrounding them with
                        angle brackets
  --ignore-images       don't include any formatting for images
  --images-to-alt       Discard image data, only keep alt text
  --images-with-size    Write image tags with height and width attrs as raw
                        html to retain dimensions
  -g, --google-doc      convert an html-exported Google Document
  -d, --dash-unordered-list
                        use a dash rather than a star for unordered list items
  -e, --asterisk-emphasis
                        use an asterisk rather than an underscore for
                        emphasized text
  -b BODY_WIDTH, --body-width=BODY_WIDTH
                        number of characters per output line, 0 for no wrap
  -i LIST_INDENT, --google-list-indent=LIST_INDENT
                        number of pixels Google indents nested lists
  -s, --hide-strikethrough
                        hide strike-through text. only relevant when -g is
                        specified as well
  --escape-all          Escape all special characters.  Output is less
                        readable, but avoids corner case formatting issues.
  --bypass-tables       Format tables in HTML rather than Markdown syntax.
  --single-line-break   Use a single line break after a block element rather
                        than two line breaks. NOTE: Requires --body-width=0
  --unicode-snob        Use unicode throughout document
  --no-automatic-links  Do not use automatic links wherever applicable
  --no-skip-internal-links
                        Do not skip internal links
  --links-after-para    Put links after each paragraph instead of document
  --mark-code           Mark program code blocks with [code]...[/code]
  --decode-errors=DECODE_ERRORS
                        What to do in case of decode errors.'ignore', 'strict'
                        and 'replace' are acceptable values

~~~
