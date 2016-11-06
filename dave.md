# dave command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
    dave [OPTIONS] URL

    E.g.

       $ dave -u pcollins -p mypass www.host.org/dav_dir/
       ...
       dave> get file.txt

    Use "dave -h" to get help on options

    Use "perldoc dave" for the whole manpage.

Options:
    -debug N
        Sets the debug level to N. 0=none. 3=noisy.

    -h  Prints basic help and options.

    -man
        Prints the full manual (equivalent to perldoc dave).

        You will need to use a pager like "more" or "less".

         e.g. dave -man |less

    -p <password>
        Sets the password to be used for the URL.

        You must also supply a user. See -u.

    -u <username>
        Sets the username to be used for the URL.

        You must also supply a pass. See -p.


~~~
