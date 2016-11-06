# tcpreplay command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

tcpreplay (tcpreplay) - Replay network traffic stored in pcap files
USAGE:  tcpreplay [ -<flag> [<val>] | --<name>[{=| }<val>] ]... <pcap_file(s)>

   -d, --dbug=num             Enable debugging output
				- it must be:  0 to 5
   -q, --quiet                Quiet mode
   -T, --timer=str            Select packet timing mode: select, ioport, rdtsc, gtod, nano, abstime
       --sleep-accel=num      Reduce the amount of time to sleep by specified usec
       --rdtsc-clicks=num     Specify the RDTSC clicks/usec
   -v, --verbose              Print decoded packets via tcpdump to STDOUT
   -A, --decode=str           Arguments passed to tcpdump decoder
				- requires these options:
				verbose
   -K, --enable-file-cache    Enable caching of packets to internal memory
				- requires these options:
				loop
       --preload-pcap         Preloads packets into RAM before sending
   -c, --cachefile=str        Split traffic via a tcpprep cache file
   -i, --intf1=str            Server/primary traffic output interface
   -I, --intf2=str            Client/secondary traffic output interface
				- requires these options:
				cachefile
       --listnics             List available network interfaces and exit
   -l, --loop=num             Loop through the capture file X times
				- it must be:  greater than or equal to 0
       --pktlen               Override the snaplen and use the actual packet len
   -L, --limit=num            Limit the number of packets to send
				- it must be:  greater than or equal to 1
   -x, --multiplier=str       Modify replay speed to a given multiple
				- prohibits these options:
				pps
				mbps
				oneatatime
				topspeed
   -p, --pps=num              Replay packets at a given packets/sec
				- prohibits these options:
				multiplier
				mbps
				oneatatime
				topspeed
   -M, --mbps=str             Replay packets at a given Mbps
				- prohibits these options:
				multiplier
				pps
				oneatatime
				topspeed
   -t, --topspeed             Replay packets as fast as possible
				- prohibits these options:
				mbps
				multiplier
				pps
				oneatatime
   -o, --oneatatime           Replay one packet at a time for each user input
				- prohibits these options:
				mbps
				pps
				multiplier
				topspeed
       --pps-multi=num        Number of packets to send for each time interval
				- requires these options:
				pps
				- it must be:  greater than or equal to 1
   -P, --pid                  Print the PID of tcpreplay at startup
       --stats=num            Print statistics every X seconds
				- it must be:  greater than or equal to 1
   -V, --version              Print version information
   -h, --less-help            Display less usage information and exit
   -H, --help                 Display usage information and exit
   -!, --more-help            Extended usage information passed thru pager
       --save-opts[=arg]      Save the option state to a config file
       --load-opts=str        Load options from a config file
				- disabled as --no-load-opts
				- may appear multiple times

Options are specified by doubled hyphens and their name
or by a single hyphen and the flag character.

tcpreplay is a tool for replaying network traffic from files saved with
tcpdump or other tools which write pcap(3) files.

The following option preset mechanisms are supported:
 - reading file /usr/bin/.tcpreplayrc

The basic operation of tcpreplay is to resend  all  packets  from  the
input file(s) at the speed at which they were recorded, or a specified 
data rate, up to as fast as the hardware is capable.

Optionally, the traffic can be split between two interfaces, written to
files, filtered and edited in various ways, providing the means to test
firewalls, NIDS and other network devices.

For more details, please see the Tcpreplay Manual at:
http://tcpreplay.synfin.net/trac/wiki/manual

~~~
