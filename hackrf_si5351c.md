# hackrf_si5351c command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
	-c, --config: print textual configuration information
	-n, --register <n>: set register number for subsequent read/write operations
	-r, --read: read register specified by last -n argument, or all registers
	-w, --write <v>: write register specified by last -n argument with value <v>
	-s, --device <s>: specify a particular device by serial number
	-d, --device <n>: specify a particular device by number

Examples:
	<command> -n 12 -r    # reads from register 12
	<command> -r          # reads all registers
	<command> -n 10 -w 22 # writes register 10 with 22 decimal
hackrf_open() failed: HACKRF_ERROR_NOT_FOUND (-5)

~~~
