# inviteflood command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


inviteflood - Version 2.0
              June 09, 2006
 Usage:
 Mandatory -
	interface (e.g. eth0)
	target user (e.g. "" or john.doe or 5000 or "1+210-555-1212")
	target domain (e.g. enterprise.com or an IPv4 address)
	IPv4 addr of flood target (ddd.ddd.ddd.ddd)
	flood stage (i.e. number of packets)
 Optional -
	-a flood tool "From:" alias (e.g. jane.doe)
	-i IPv4 source IP address [default is IP address of interface]
	-S srcPort  (0 - 65535) [default is well-known discard port 9]
	-D destPort (0 - 65535) [default is well-known SIP port 5060]
	-l lineString line used by SNOM [default is blank]
	-s sleep time btwn INVITE msgs (usec)
	-h help - print this usage
	-v verbose output mode


~~~
