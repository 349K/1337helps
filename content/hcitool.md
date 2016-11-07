# hcitool command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

hcitool - HCI Tool ver 5.36
Usage:
	hcitool [options] <command> [command parameters]
Options:
	--help	Display help
	-i dev	HCI device
Commands:
	dev 	Display local devices
	inq 	Inquire remote devices
	scan	Scan for remote devices
	name	Get name from remote device
	info	Get information from remote device
	spinq	Start periodic inquiry
	epinq	Exit periodic inquiry
	cmd 	Submit arbitrary HCI commands
	con 	Display active connections
	cc  	Create connection to remote device
	dc  	Disconnect from remote device
	sr  	Switch master/slave role
	cpt 	Change connection packet type
	rssi	Display connection RSSI
	lq  	Display link quality
	tpl 	Display transmit power level
	afh 	Display AFH channel map
	lp  	Set/display link policy settings
	lst 	Set/display link supervision timeout
	auth	Request authentication
	enc 	Set connection encryption
	key 	Change connection link key
	clkoff	Read clock offset
	clock	Read local or remote clock
	lescan	Start LE scan
	leinfo	Get LE remote information
	lewladd	Add device to LE White List
	lewlrm	Remove device from LE White List
	lewlsz	Read size of LE White List
	lewlclr	Clear LE White List
	lerladd	Add device to LE Resolving List
	lerlrm	Remove device from LE Resolving List
	lerlclr	Clear LE Resolving List
	lerlsz	Read size of LE Resolving List
	lerlon	Enable LE Address Resolution
	lerloff	Disable LE Address Resolution
	lecc	Create a LE Connection
	ledc	Disconnect a LE Connection
	lecup	LE Connection Update

For more information on the usage of each command use:
	hcitool <command> --help

~~~
