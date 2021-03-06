# sakis3g command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Sakis 3G All-in-one script - Version 0.2.0e
(c) Sakis Dimopoulos 2009, 2010 under GNU GPL v2


Usage:
      sakis3g [actors] [switches] [variables]

Sakis3G is a shell script which is supposed to work out-of-the-box for 
establishing a 3G connection with any combination of modem or operator. 

NOTE: This script requires root priviledges to properly work. If not executed 
from root, it will try to acquire them.

Common actors are:
connect       - Attempts to establish 3G connection.
disconnect    - Stops all active PPP connections.
toggle        - Attempts to establish 3G connection. If already connected, it 
disconnects instead.
reconnect     - Attempts to establish 3G connection. If already connected, it 
first disconnects and then attempts.
start         - Same as connect. Provided for use as init.d script.
stop          - Same as disconnect. Provided for use as init.d script.
reload        - Same as reconnect. Provided for use as init.d script.
force-reload  - Same as reload. Provided for use as init.d script.
restart       - Same as reload. Provided for use as init.d script.
desktop       - Creates desktop shortcut for this script.
status        - Prints connection status and exits. Exit code is 0 if 
connected, or 6 if not connected.
help          - Prints this screen and exits.
man           - Displays man page.

NOTE: For more information, you should consult man page or official Sakis3G 
wiki, available at:
  http://wiki.sakis3g.org/


~~~
