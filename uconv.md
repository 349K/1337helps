# uconv command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: uconv [ -h, -?, --help ] [ -V, --version ] [ -s, --silent ] [ -v, --verbose ] [ -l, --list | --list-code code | --default-code | -L, --list-transliterators ] [ --canon ] [ -x transliteration ] [ --to-callback callback | -c ] [ --from-callback callback | -i ] [ --callback callback ] [ --fallback | --no-fallback ] [ -b, --block-size size ] [ -f, --from-code code ] [ -t, --to-code code ] [ --add-signature ] [ --remove-signature ] [ -o, --output file ] [ file ... ]

Options:  -h, --help                    print this message
          -V, --version                 print the program version
          -s, --silent                  suppress messages
          -v, --verbose                 display progress information
          -l, --list                    list all available encodings
          --list-code code              list only the given encoding
          --default-code                list only the default encoding
          -L, --list-transliterators    list all available transliterators
          --canon                       print list in cnvrtrs.txt(5) format
          -x transliteration            run everything through transliteration
          --to-callback callback        use callback on destination encoding
          -c                            omit invalid characters from the output
          --from-callback callback      use callback on original encoding
          -i                            ignore invalid sequences in the input
          --callback callback           use callback on both encodings
          -b, --block-size size         read size bytes blocks (default: 4096)
          --fallback                    use fallback mapping
          --no-fallback                 do not use fallback mapping
          -f, --from-code code          set the original encoding
          -t, --to-code code            set the destination encoding
          --add-signature               add a U+FEFF Unicode signature character (BOM)
          --remove-signature            remove a U+FEFF Unicode signature character (BOM)
          -o, --output file             write output to file

Callbacks: substitute skip stop escape escape-icu escape-java escape-c escape-xml escape-xml-hex escape-xml-dec escape-unicode

~~~
