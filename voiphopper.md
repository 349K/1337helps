# voiphopper command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

VoIP Hopper Extended Usage:

Miscellaneous Options:
	-l (list available interfaces for CDP sniffing, then exit)
	Example:  voiphopper -l
	-m (Spoof the MAC Address, then exit)
	Example:  voiphopper -i eth0 -m 00:07:0E:EA:50:86
	-d (Delete the VLAN Interface, then exit)
	Example:  voiphopper -d eth0.200
	-V (Print the VoIP Hopper version, then exit)
	Example:  voiphopper -V

MAC Address Spoofing Options (used with -a, -v, or -c options):
	-m (Spoof the MAC Address of existing interface, and new Interface)
	-D -m (Spoof the MAC Address of only new Voice Interface)
	Example:  voiphopper -i eth0 -m 00:07:0E:EA:50:86
	Example:  voiphopper -i eth0 -D -m 00:07:0E:EA:50:86

CDP Sniff Mode (-c 0)
	Example:  voiphopper -i eth0 -c 0

CDP Spoof Mode (-c 1):
	-E <string> (Device ID)
	-P <string> (Port ID)
	-C <string> (Capabilities)
	-L <string> (Platform)
	-S <string> (Software)
	-U <string> (Duplex)

Example Usage for SIP Firmware Phone:
voiphopper -i eth0 -c 1 -E 'SIP00070EEA5086' -P 'Port 1' -C Host -L 'Cisco IP Phone 7940' -S 'P003-08-8-00' -U 1

Example Usage for SCCP Firmware Phone:
voiphopper -i eth0 -c 1 -E 'SEP0070EEA5086' -P 'Port 1' -C Host -L 'Cisco IP Phone 7940' -S 'P00308000700' -U 1

Example Usage for Phone with MAC Spoofing:
voiphopper -i eth0 -m 00:07:0E:EA:50:86 -c 1 -E 'SEP00070EEA5086' -P 'Port 1' -C Host -L 'Cisco IP Phone 7940' -S 'P003-08-8-00' -U 1

Avaya DHCP Option Mode (-a):
	Example:  voiphopper -i eth0 -a
	Example:  voiphopper -i eth0 -a -m 00:07:0E:EA:50:86

VLAN Hop Mode (-v VLAN ID):
	Example:  voiphopper -i eth0 -v 200
	Example:  voiphopper -i eth0 -v 200 -D -m 00:07:0E:EA:50:86

Alcatel VLAN Discovery (-t 0|1|2):
	Example:  voiphopper -i eth0 -t 0
	Example:  voiphopper -i eth0 -t 1
	Example:  voiphopper -i eth0 -t 0 -m 00:80:9f:ad:42:42
	Example:  voiphopper -i eth0 -t 1 -m 00:80:9f:ad:42:42
	Example:  voiphopper -i eth0 -t 2 -v 800
	Example:  voiphopper -i eth0 -t 2 -v 800 -m 00:80:9f:ad:42:42


~~~
