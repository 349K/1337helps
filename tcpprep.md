# tcpprep command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

tcpprep (tcpprep) - Create a tcpreplay cache cache file from a pcap file.
USAGE:  tcpprep [ -<flag> [<val>] | --<name>[{=| }<val>] ]...

   -d, --dbug=num             Enable debugging output
				- it must be:  0 to 5
   -a, --auto=str             Auto-split mode
				- prohibits these options:
				cidr
				port
				regex
				mac
   -c, --cidr=str             CIDR-split mode
				- prohibits these options:
				auto
				port
				regex
				mac
   -r, --regex=str            Regex-split mode
				- prohibits these options:
				auto
				port
				cidr
				mac
   -p, --port                 Port-split mode
				- prohibits these options:
				auto
				regex
				cidr
				mac
   -e, --mac=str              Source MAC split mode
				- prohibits these options:
				auto
				regex
				cidr
				port
       --reverse              Matches to be client instead of server
   -C, --comment=str          Embeded cache file comment
       --no-arg-comment       Do not embed any cache file comment
   -x, --include=str          Include only packets matching rule
				- prohibits these options:
				exclude
   -X, --exclude=str          Exclude any packet matching this rule
				- prohibits these options:
				include
   -o, --cachefile=str        Output cache file
   -i, --pcap=str             Input pcap file to process
   -P, --print-comment=str    Print embedded comment in the specified cache file
   -I, --print-info=str       Print basic info from the specified cache file
   -S, --print-stats=str      Print statistical information about the specified cache file
   -s, --services=str         Load services file for server ports
				- requires these options:
				port
   -N, --nonip                Send non-IP traffic out server interface
   -R, --ratio=str            Ratio of client to server packets
				- requires these options:
				auto
   -m, --minmask=num          Minimum network mask length in auto mode
				- requires these options:
				auto
				- it must be:  0 to 32
   -M, --maxmask=num          Maximum network mask length in auto mode
				- requires these options:
				auto
				- it must be:  0 to 32
   -v, --verbose              Print decoded packets via tcpdump to STDOUT
   -A, --decode=str           Arguments passed to tcpdump decoder
				- requires these options:
				verbose
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

tcpprep is a ``pcap(3)'' file pre-processor which creates a cache
file which provides "rules" for ``tcprewrite(1)'' and ``tcpreplay(1)''
on how to process and send packets.

The following option preset mechanisms are supported:
 - reading file /usr/bin/.tcppreprc

The basic operation of tcpreplay is to resend all packets from the
input file(s) out a single file.  Tcpprep processes a pcap file and 
applies a set of user-specified rules to create a cache file which 
tells tcpreplay wether or not to send each packet and which interface the
packet should be sent out of.

For more details, please see the Tcpreplay Manual at:
http://tcpreplay.synfin.net/trac/wiki/manual

~~~
