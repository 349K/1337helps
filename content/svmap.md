# svmap command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: svmap [options] host1 host2 hostrange
Scans for SIP devices on a given network

examples:

svmap 10.0.0.1-10.0.0.255 172.16.131.1 sipvicious.org/22 10.0.1.1/241.1.1.1-20 1.1.2-20.* 4.1.*.*

svmap -s session1 --randomize 10.0.0.1/8

svmap --resume session1 -v

svmap -p5060-5062 10.0.0.3-20 -m INVITE



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
  --randomscan          Scan random IP addresses
  -i scan1, --input=scan1
                        Scan IPs which were found in a previous scan. Pass the
                        session name as the argument
  -I scan1, --inputtext=scan1
                        Scan IPs from a text file - use the same syntax as
                        command line but with new lines instead of commas.
                        Pass the file name as the argument
  -m METHOD, --method=METHOD
                        Specify the request method - by default this is
                        OPTIONS.
  -d, --debug           Print SIP messages received
  --first=FIRST         Only send the first given number of messages (i.e.
                        usually used to scan only X IPs)
  -e EXTENSION, --extension=EXTENSION
                        Specify an extension - by default this is not set
  --randomize           Randomize scanning instead of scanning consecutive ip
                        addresses
  --srv                 Scan the SRV records for SIP on the destination domain
                        name.The targets have to be domain names - example.org
                        domain1.com
  --fromname=FROMNAME   specify a name for the from header

~~~
