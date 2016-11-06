# mech-dump command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
    mech-dump [options] [file|url]

    Options:

        --headers              Dump HTTP response headers
        --forms                Dump table of forms (default action)
        --links                Dump table of links
        --images               Dump table of images
        --all                  Dump all four of the above, in that order

        --text                 Dumps the textual part of the web page

        --user=user            Set the username
        --password=pass        Set the password
        --cookie-file=filename Set the filename to use for persistent cookies

        --agent=agent          Specify the UserAgent to pass
        --agent-alias=alias
                               Specify the alias for the UserAgent to pass.
                               Pick one of:
                                   * Windows IE 6
                                   * Windows Mozilla
                                   * Mac Safari
                                   * Mac Mozilla
                                   * Linux Mozilla
                                   * Linux Konqueror

        --absolute             Show URLs as absolute, even if relative in the page
        --help                 Show this message

    The order of the options specified is relevant. Repeated options get
    repeated dumps.

    Proxy settings are specified through the environment (e.g.
    "http_proxy=http://proxy.my.place/"). See LWP::UserAgent for details.


~~~
