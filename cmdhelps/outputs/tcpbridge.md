# tcpbridge command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

tcpbridge (tcpbridge) - Bridge network traffic across two interfaces
USAGE:  tcpbridge [ -<flag> [<val>] | --<name>[{=| }<val>] ]...




   -r, --portmap=str          Rewrite TCP/UDP ports
				- may appear multiple times
   -s, --seed=num             Randomize src/dst IPv4/v6 addresses w/ given seed
   -N, --pnat=str             Rewrite IPv4/v6 addresses using pseudo-NAT
				- prohibits these options:
				srcipmap
				- may appear up to 2 times
   -S, --srcipmap=str         Rewrite source IPv4/v6 addresses using pseudo-NAT
				- prohibits these options:
				pnat
   -D, --dstipmap=str         Rewrite destination IPv4/v6 addresses using pseudo-NAT
				- prohibits these options:
				pnat
   -b, --skipbroadcast        Skip rewriting broadcast/multicast IPv4/v6 addresses
   -C, --fixcsum              Force recalculation of IPv4/TCP/UDP header checksums
   -m, --mtu=num              Override default MTU length (1500 bytes)
				- it must be:  1 to 65549
       --mtu-trunc            Truncate packets larger then specified MTU
   -E, --efcs                 Remove Ethernet checksums (FCS) from end of frames
       --ttl=str              Modify the IPv4/v6 TTL/Hop Limit
       --tos=num              Set the IPv4 TOS/DiffServ/ECN byte
				- it must be:  0 to 255
       --tclass=num           Set the IPv6 Traffic Class byte
				- it must be:  0 to 255
       --flowlabel=num        Set the IPv6 Flow Label
				- it must be:  0 to 1048575
   -F, --fixlen=str           Pad or truncate packet data to match header length
       --skipl2broadcast      Skip rewriting broadcast/multicast Layer 2 addresses
       --dlt=str              Override output DLT encapsulation
       --enet-dmac=str        Override destination ethernet MAC addresses
       --enet-smac=str        Override source ethernet MAC addresses
       --enet-vlan=str        Specify ethernet 802.1q VLAN tag mode
       --enet-vlan-tag=num    Specify the new ethernet 802.1q VLAN tag value
				- requires these options:
				enet-vlan
				- it must be:  0 to 4095
       --enet-vlan-cfi=num    Specify the ethernet 802.1q VLAN CFI value
				- requires these options:
				enet-vlan
				- it must be:  0 to 1
       --enet-vlan-pri=num    Specify the ethernet 802.1q VLAN priority
				- requires these options:
				enet-vlan
				- it must be:  0 to 7
       --hdlc-control=num     Specify HDLC control value
       --hdlc-address=num     Specify HDLC address
       --user-dlt=num         Set output file DLT type
       --user-dlink=str       Rewrite Data-Link layer with user specified data
				- may appear up to 2 times
   -d, --dbug=num             Enable debugging output
				- it must be:  0 to 5
   -i, --intf1=str            Primary interface (listen in uni-directional mode)
   -I, --intf2=str            Secondary interface (send in uni-directional mode)
   -u, --unidir               Send and receive in only one direction
       --listnics             List available network interfaces and exit
   -L, --limit=num            Limit the number of packets to send
				- it must be:  greater than or equal to 1
   -M, --mac=str              MAC addresses of local NIC's
				- may appear up to 2 times
   -x, --include=str          Include only packets matching rule
				- prohibits these options:
				exclude
   -X, --exclude=str          Exclude any packet matching this rule
				- prohibits these options:
				include
   -P, --pid                  Print the PID of tcpbridge at startup
   -v, --verbose              Print decoded packets via tcpdump to STDOUT
   -A, --decode=str           Arguments passed to tcpdump decoder
				- requires these options:
				verbose
   -V, --version              Print version information
   -h, --less-help            Display less usage information and exit

version and help options:

   -H, --help                 Display usage information and exit
   -!, --more-help            Extended usage information passed thru pager
   --, --save-opts[=arg]      Save the option state to a config file
   -., --load-opts=str        Load options from a config file
				- disabled as --no-load-opts
				- may appear multiple times

Options are specified by doubled hyphens and their name
or by a single hyphen and the flag character.

tcpbridge is a tool for selectively briding network traffic across two interfaces
and optionally modifying the packets in betweeen

The following option preset mechanisms are supported:
 - reading file /usr/bin/.tcpbridgerc

The basic operation of tcpbridge is to be a network bridge between two
subnets.  All packets received on one interface are sent via the other.

Optionally, packets can be edited in a variety of ways according to your needs.

For more details, please see the Tcpreplay Manual at:
http://tcpreplay.synfin.net/trac/wiki/manual

~~~
