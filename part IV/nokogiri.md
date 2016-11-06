# nokogiri command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Nokogiri: an HTML, XML, SAX, and Reader parser
Usage: nokogiri <uri|path> [options]

Examples:
  nokogiri https://www.ruby-lang.org/
  nokogiri ./public/index.html
  curl -s http://www.nokogiri.org | nokogiri -e'p $_.css("h1").length'

Options:
        --type type                  Parse as type: xml or html (default: auto)
    -C file                          Specifies initialization file to load (default /root/.nokogirirc)
    -E, --encoding encoding          Read as encoding (default: none)
    -e command                       Specifies script from command-line.
        --rng <uri|path>             Validate using this rng file.
    -?, --help                       Show this message
    -v, --version                    Show version

~~~
