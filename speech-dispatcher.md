# speech-dispatcher command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: speech-dispatcher [-{d|s}] [-l {1|2|3|4|5}] [-c com_method] [-S socket_path] [-p port] [-t timeout] | [-v] | [-h]
Speech Dispatcher -- Common interface for Speech Synthesis (GNU GPL)

-d, --run-daemon	Run as a daemon
-s, --run-single	Run as single application
-a, --spawn		Start only if autospawn is not disabled
-l, --log-level		Set log level (between 1 and 5)
-L, --log-dir		Set path to logging
-c, --communication-method	Communication method to use ('unix_socket' or 'inet_socket')
-S, --socket-path	Socket path to use for 'unix_socket' method (filesystem path or 'default')
-p, --port		Specify a port number for 'inet_socket' method
-t, --timeout		Set time in seconds for the server to wait before it shuts down,
			if it has no clients connected
-P, --pid-file		Set path to pid file
-C, --config-dir	Set path to configuration
-m, --module-dir	Set path to modules
-v, --version		Report version of this program
-D, --debug		Output debugging information into $TMPDIR/speechd-debug if TMPDIR is exported, otherwise to /tmp/speechd-debug
-h, --help		Print this info

Copyright (C) 2002-2012 Brailcom, o.p.s.
This is free software; you can redistribute it and/or modify it
under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2, or (at your option)
any later version. Please see COPYING for more details.

Please report bugs to speechd@lists.freebsoft.org


~~~
