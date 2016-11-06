# gpg-connect-agent command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


gpg-connect-agent (GnuPG) 2.1.11
Copyright (C) 2016 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

Home: ~/.gnupg

Syntax: gpg-connect-agent [options]
Connect to a running agent and send commands


Options:
 
 -v, --verbose           verbose
 -q, --quiet             quiet
     --hex               print data out hex encoded
     --decode            decode received data lines
     --dirmngr           connect to the dirmngr
 -S, --raw-socket NAME   connect to Assuan socket NAME
 -T, --tcp-socket ADDR   connect to Assuan server at ADDR
 -E, --exec              run the Assuan server given on the command line
     --no-ext-connect    do not use extended connect mode
 -r, --run FILE          run commands from FILE on startup
 -s, --subst             run /subst on startup

Please report bugs to <http://bugs.gnupg.org>.

~~~
