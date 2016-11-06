# querybts command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: querybts [options] {<package> | <report number> [report2] ...}

querybts - Examine the state of a debbugs server.

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -A, --archive         Browse archived bugs.
  -b, --buglist         Display a bugs list for the given package.
  -B SYSTEM, --bts=SYSTEM
                        Specify an alternate debbugs BTS; available values:
                        debian
  -m, --mbox            generate mbox
  --proxy=HTTP_PROXY, --http_proxy=HTTP_PROXY
                        define the proxy to use
  -s, --source          Query for source packages rather than binary packages.
  --timeout=TIMEOUT     Specify the network timeout, in seconds [default: 60].
  -u INTERFACE, --ui=INTERFACE, --interface=INTERFACE
                        Specify the user interface to use; available values:
                        text, urwid, gtk2
  -w, --web             Use a web browser instead of the internal interface.
  --mbox-reader-cmd=MBOX_READER_CMD
                        Specify the program to open the reports mbox.
  --latest-first        Order bugs to show the latest first

~~~
