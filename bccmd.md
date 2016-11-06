# bccmd command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

bccmd - Utility for the CSR BCCMD interface

Usage:
	bccmd [options] <command>

Options:
	-t <transport>     Select the transport
	-d <device>        Select the device
	-b <bcsp rate>     Select the bcsp transfer rate
	-h, --help         Display help

Transports:
	HCI USB BCSP H4 3WIRE

Commands:
	builddef                       	Get build definitions
	keylen     <handle>            	Get current crypt key length
	clock                          	Get local Bluetooth clock
	rand                           	Get random number
	chiprev                        	Get chip revision
	buildname                      	Get the full build name
	panicarg                       	Get panic code argument
	faultarg                       	Get fault code argument
	coldreset                      	Perform cold reset
	warmreset                      	Perform warm reset
	disabletx                      	Disable TX on the device
	enabletx                       	Enable TX on the device
	singlechan <channel>           	Lock radio on specific channel
	hoppingon                      	Revert to channel hopping
	rttxdata1  <freq> <level>      	TXData1 radio test
	radiotest  <freq> <level> <id> 	Run radio tests
	memtypes                       	Get memory types
	psget      <key>               	Get value for PS key
	psset      <key> <value>       	Set value for PS key
	psclr      <key>               	Clear value for PS key
	pslist                         	List all PS keys
	psread                         	Read all PS keys
	psload     <file>              	Load all PS keys from PSR file
	pscheck    <file>              	Check PSR file
	adc        <mux>               	Read ADC value of <mux> input

Keys:
	bdaddr country devclass keymin keymax features commands version 
	remver hciextn mapsco baudrate hostintf anafreq anaftrim usbvid 
	usbpid dfupid bootmode 

~~~
