# sbd command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


sbd 1.37 Copyright (C) 2004 Michel Blomgren <michel.blomgren@tigerteam.se>
$Id: sbd.c,v 1.37 2005/08/21 22:40:47 shadow Exp $

This program is free software; you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation; either version 2 of the License, or (at your option) any later
version.

connect (tcp): sbd [-options] host port
listen (tcp):  sbd -l -p port [-options]
options:
    -l          listen for incoming connection
    -p n        choose port to listen on, or source port to connect out from
    -a address  choose an address to listen on or connect out from
    -e prog     program to execute after connect (e.g. -e cmd.exe or -e bash)
    -r n        infinitely respawn/reconnect, pause for n seconds between
                connection attempts. -r0 can be used to re-listen after
                disconnect (just like a regular daemon)
    -c on|off   encryption on/off. specify whether you want to use the built-in
                AES-CBC-128 + HMAC-SHA1 encryption implementation (by
                Christophe Devine - http://www.cr0.net:8040/) or not
                default is: -c on
    -k secret   override default phrase to use for encryption (secret must be
                shared between client and server)
    -q          hush, quiet, don't print anything (overrides -v)
    -v          be verbose
    -n          toggle numeric-only IP addresses (don't do DNS resolution). if
                you specify -n twice, original state will be active (i.e. -n
                works like a on/off switch)
    -m          toggle monitoring (snooping) on/off (only used with the -e
                option). snooping can also be turned on by specifying -vv (-v
                two times)
    -P prefix   add prefix (+ a hardcoded separator) to all outbound data.
                this option is mostly only useful for sbd in "chat mode" (to
                prefix lines you send with your nickname)
    -H on|off   highlight incoming data with a hardcoded (color) escape
                sequence (for e.g. chatting). default is: -H off
    -V          print version banner and exit (include that output in your
                bug report and send bug report to michel.blomgren@tigerteam.se)
unix-like OS specific options:
    -s          invoke a shell, nothing else. if sbd is setuid 0, it'll invoke
                a root shell
    -w n        "immobility timeout" in seconds for idle read/write operations
                and program execution (the -e option)
    -D on|off   fork and run in background (daemonize). default: -D off

~~~
