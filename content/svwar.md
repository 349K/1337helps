# svwar command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: svwar [options] target
examples:
svwar -e100-999 10.0.0.1
svwar -d dictionary.txt 10.0.0.2


Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -v, --verbose         Increase verbosity
  -q, --quiet           Quiet mode
  -p PORT, --port=PORT  Destination port or port ranges of the SIP device - eg
                        -p5060,5061,8000-8100
  -P PORT, --localport=PORT
                        Source port for our packets
  -x IP, --externalip=IP
                        IP Address to use as the external ip. Specify this if
                        you have multiple interfaces or if you are behind NAT
  -b BINDINGIP, --bindingip=BINDINGIP
                        By default we bind to all interfaces. This option
                        overrides that and binds to the specified ip address
  -t SELECTTIME, --timeout=SELECTTIME
                        This option allows you to trottle the speed at which
                        packets are sent. Change this if you're losing
                        packets. For example try 0.5.
  -R, --reportback      Send the author an exception traceback. Currently
                        sends the command line parameters and the traceback
  -A, --autogetip       Automatically get the current IP address. This is
                        useful when you are not getting any responses back due
                        to SIPVicious not resolving your local IP.
  -s NAME, --save=NAME  save the session. Has the benefit of allowing you to
                        resume a previous scan and allows you to export scans
  --resume=NAME         resume a previous scan
  -c, --enablecompact   enable compact mode. Makes packets smaller but
                        possibly less compatible
  -d DICTIONARY, --dictionary=DICTIONARY
                        specify a dictionary file with possible extension
                        names
  -m OPTIONS, --method=OPTIONS
                        specify a request method. The default is REGISTER.
                        Other possible methods are OPTIONS and INVITE
  -e RANGE, --extensions=RANGE
                        specify an extension or extension range  example: -e
                        100-999,1000-1500,9999
  -z PADDING, --zeropadding=PADDING
                        the number of zeros used to padd the username.
                        the options "-e 1-9999 -z 4" would give 0001 0002 0003
                        ... 9999
  --force               Force scan, ignoring initial sanity checks.
  -T TEMPLATE, --template=TEMPLATE
                        A format string which allows us to specify a template
                        for the extensions                       example
                        svwar.py -e 1-999 --template="123%#04i999" would scan
                        between 1230001999 to 1230999999"
  -D, --enabledefaults  Scan for default / typical extensions such as
                        1000,2000,3000 ... 1100, etc. This option is off by
                        default.                       Use --enabledefaults to
                        enable this functionality
  --maximumtime=MAXIMUMTIME
                        Maximum time in seconds to keep sending requests
                        without                       receiving a response
                        back
  --domain=DOMAIN       force a specific domain name for the SIP message, eg.
                        -d example.org
  --debug               Print SIP messages received

~~~
